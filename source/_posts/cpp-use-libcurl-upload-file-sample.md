---
title: C++使用libcurl上传文件代码示例
id: 1323
categories:
  - 未分类
date: 2014-07-03 18:38:50
tags:
---

```cpp
#include <stdio.h>
#include <iostream>
#include <string>

#define CURL_STATICLIB
#include "curl/curl.h"

//简单的post请求示例
void post_simple()
{
  /* get a curl handle */
  CURL *curl = curl_easy_init();
  if(curl) {
    /* First set the URL that is about to receive our POST. This URL can
       just as well be a https:// URL if that is what should receive the
       data. */
    curl_easy_setopt(curl, CURLOPT_PROXY, "172.18.172.251:80");
	  curl_easy_setopt(curl, CURLOPT_URL, "http://radaronline.sinaapp.com/post.php?fa=po");
    /* Now specify the POST data */
    curl_easy_setopt(curl, CURLOPT_POSTFIELDS, "name=daniel&project=curl");

    /* Perform the request, res will get the return code */
    CURLcode res = curl_easy_perform(curl);
    /* Check for errors */
    if(res != CURLE_OK)
      fprintf(stderr, "curl_easy_perform() failed: %s\n",
              curl_easy_strerror(res));

    /* always cleanup */
    curl_easy_cleanup(curl);
  }

}

//自定义处理函数 注册后libcurl将调用此函数处理接收到的数据
size_t write_data(void *buffer, size_t size, size_t nmemb, void *userp) {
    FILE *fptr = (FILE*)userp;
    fwrite(buffer, size, nmemb, fptr);

	printf("nmemb:%d, size:%d",nmemb, size);
	return nmemb*size;//必须返回实际处理的字节数 否则curl将认为处理失败
}

//自定义处理函数 简单演示将数据输出到控制台
size_t write_console(void *buffer, size_t size, size_t count, void *userp) {

	std::string str((const char*)buffer, size*count);

	std::cout<<str;
	return count*size;
}

//文件上传示例
void post_file()
{
	const char* POSTURL =  "http://radaronline.sinaapp.com/post.php?fa=po";

	//const char* FILENAME =  "a.txt";

	//FILE *fptr;

	//if ((fptr = fopen(FILENAME, "w")) == NULL) {//for receive response data
	//	fprintf(stderr, "fopen file error: %s\n", FILENAME);
	//	exit(1);
	//}

	CURL *curl = curl_easy_init();

	curl_easy_setopt(curl, CURLOPT_PROXY, "172.18.172.251:80");//设置代理 如不需要可注释此行

        //设置自定义处理函数 不设置时默认将接收到的数据输出到控制台
	curl_easy_setopt(curl, CURLOPT_WRITEFUNCTION, write_console);

        //设置输出到文件的文件指针 	
        //curl_easy_setopt(curl, CURLOPT_WRITEDATA, fptr);

	curl_httppost *formpost = 0, *lastptr  = 0;//指向表单链表的首尾

	curl_formadd(&formpost, &lastptr, CURLFORM_PTRNAME, "reqformat", CURLFORM_PTRCONTENTS, "plain", CURLFORM_END);
	curl_formadd(&formpost, &lastptr, CURLFORM_PTRNAME, "file", CURLFORM_FILE, "b.txt", CURLFORM_END);
	curl_easy_setopt(curl, CURLOPT_URL, POSTURL);
	curl_easy_setopt(curl, CURLOPT_HTTPPOST, formpost);

        //发送请求
	CURLcode res = curl_easy_perform(curl);

	curl_easy_cleanup(curl);
}

int main(void)
{	  /* In windows, this will init the winsock stuff */
	curl_global_init(CURL_GLOBAL_ALL);

	post_file();

	curl_global_cleanup();
	return 0;
}
```