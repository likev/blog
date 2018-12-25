---
title: NCEP FNL 介绍
id: 952
categories:
  - 未分类
date: 2011-10-31 17:42:44
tags:
---

>[原文链接] [dss.ucar.edu/datasets/ds083.2/](http://dss.ucar.edu/datasets/ds083.2/)

<span style="font-size: medium;">**SUPPLEMENTARY DOCUMENTATION**</span>

Background information about this type of data may be found in [ An Introduction to Atmospheric and Oceanographic Datasets](http://dss.ucar.edu/docs/data-intro-technote/).

**INFORMATION ABOUT THE NCEP GDAS FNL 1.0 DEGREE 6-HOURLY ANALYSIS UPDATES**

The CISL/DSS archived FNL analysis filenames have the form fnl_yymmdd_hh_00[_c] , the yymmdd_hh is in Coordinated Universal Time (UTC, UT, GMT or Z). The _00 in this form indicates that the file is an analysis, not a forecast. Files published on the CISL/DSS web site are grib1\. Beginning 2008.09.30.12, when filename is appended with "_c", it means CISL/DSS converted it from grib2 to grib1.

The CISL/DSS FNL files originated as downloads of the near-real time analysis files on an NCEP Nomads server directory: http://nomads.ncep.noaa.gov/pub/data/nccf/com/gfs/prod/gdas.YYYYMMDD , and the files are named gdas1.thhz.pgrbf00.grib2 where hh is the analysis time and f00 indicates an analysis.  pgrb files with other fnn values are forecasts nn hours into the future.  Numerous other files are in these directories.  The NCEP directories are emptied after about 30 hours, and aged off after about 48 hours.

CISL/DSS selects the FNL analysis over all others because it uses the most complete set of observations and is run last in the sequence of operational global models.  The FNL is likely the best option for a long-term operational model archive from NCEP. Please see the NCEP [EMC Model Documentation](http://www.emc.ncep.noaa.gov/modelinfo/index.html) for more details.

As with any high volume operational model production system there are times when late file postings and network outages interrupt data acquisition and processing for the archive.  The CISL/DSS makes a "best" effort to sustain a complete archive time series.  Recoveries from short-term problems are handled systematically.  For longer-term problems we obtain assistance from NCEP staff.

<span style="color: brown; font-size: medium;">**VARIABLES:**</span>

Land skin temperature and sea surface temperature are in one field.

<span style="color: brown; font-size: medium;">**LEVELS:**</span>
1000mb 975mb 925mb 900mb 850mb 800mb 700mb 650mb 600mb 550mb 500mb 450mb 400mb 350mb 300mb 250mb 200mb 150mb 100mb 70mb 50mb 30mb 20mb 10mb
surface upper-air troposphere mandatory tropopause stratosphere

<span style="color: brown; font-size: medium;">**FORMAT AND USAGE:**</span>

**General**

To see the WMO's GRIB Documentation click [<span style="color: red;">here</span>](http://dss.ucar.edu/docs/formats/grib/gribdoc/).
To see NCEP's GRIB1 Documentation click [<span style="color: red;">here</span>](http://www.nco.ncep.noaa.gov/pmb/codes/GRIB1/).
To see NCEP's GRIB2 Documentation click [<span style="color: red;">here</span>](http://www.nco.ncep.noaa.gov/pmb/docs/grib2/).
To see FAQs about FNL and ADP data click [<span style="color: red;">here</span>](http://dss.ucar.edu/faqs/using.html#msgdata).

**Tools to manipulate GRIB data**

For support using NCAR/CISL's NCL click [<span style="color: red;">here</span>](http://www.ncl.ucar.edu/overview.shtml).
For support using COLA's GrADS click [<span style="color: red;">here</span>](http://grads.iges.org/grads/).

**Models**

For support using NCAR/MMM's WRF click [<span style="color: red;">here</span>](http://www.mmm.ucar.edu/wrf/users/support.html).
For support using NCAR/MMM's MM5 click [<span style="color: red;">here</span>](http://www.mmm.ucar.edu/mm5/support.html).
For support using ATMET's RAMS click [<span style="color: red;">here</span>](http://www.atmet.com/).
