---
title: C++ 以POST方式向网页提交数据
tags:
  - C++
  - post
  - 代码
  - 网页
  - 请求
id: 993
categories:
  - C++
date: 2011-11-10 11:21:24
---

示例代码如下：
<pre lang='cpp'>

#include <iostream>
#include <string>
#include <afxinet.h> //定义了MFC CInternetSession类等

bool PostHttpPage(const std::string& hostName, const std::string& pathName, const std::string& postData)
{
	using namespace std;

	CInternetSession session("your app agent name");

	try
	{
		INTERNET_PORT nPort = 80;
		DWORD dwRet = 0;

		CHttpConnection* pServer = session.GetHttpConnection(hostName.c_str(), nPort);
		CHttpFile* pFile = pServer->OpenRequest(CHttpConnection::HTTP_VERB_POST, pathName.c_str());

		CString strHeaders = "Content-Type: application/x-www-form-urlencoded"; // 请求头

		//开始发送请求

		pFile->SendRequest(strHeaders,(LPVOID)postData.c_str(),postData.size());
		pFile->QueryInfoStatusCode(dwRet);

		if (dwRet == HTTP_STATUS_OK)
		{
			CString result, newline;

			while(pFile->ReadString(newline))
			{//循环读取每行内容
				result += newline+"\r\n";
			}

			std::cout<<result<<std::endl;//显示返回内容
		}
		else
		{
			return false;
		}
		delete pFile;
		delete pServer;

	}
	catch (CInternetException* pEx)
	{
		//catch errors from WinInet
		TCHAR pszError[200];
		pEx->GetErrorMessage(pszError, 200);

		std::cout<<pszError<<std::endl;//显示异常信息
		return false;
	}
	session.Close();

	return true;
}

int main(void)
{
	//向http://current.sinaapp.com/post.php发送数据
	PostHttpPage("current.sinaapp.com","post.php","name=rain&age=12");
}
</pre>