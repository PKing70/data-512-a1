# Data Curation
Data 512 [Assignment 1](https://wiki.communitydata.cc/Human_Centered_Data_Science_(Fall_2018)/Assignments#A1:_Data_curation): Data Curation

University of Washington DATA 512

Instructors Morgan and Keyes

## Goal

To acquire, process, and analyze data using open research best practices, I was tasked with obtaining site traffic data from Wikimedia APIs and delivering the resulting data and graph files in this repository.

## Licenses and Terms of Use

The source data is [CC0 1.0 licensed](https://creativecommons.org/publicdomain/zero/1.0/), and usage should follow the mediawiki [terms and conditions of use](https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions).
The code in this repository is [MIT licensed](https://opensource.org/licenses/MIT).

## APIs

The Legacy [Pagecounts](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts) API provides access to desktop and mobile traffic data from December 2007 through July 2016.
The [Pageviews](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews) API provides access to desktop, mobile web, and mobile app traffic data from July 2015 through last month.

## Data

### Files

The data files in this repository are:

|File|Description|
|---|---|
|README.md|[Overview](https://wiki.communitydata.cc/Human_Centered_Data_Science_(Fall_2018)/Assignments#Step_4:_Documentation) of project. Start here! |
|LICENSE|MIT to cover the files in this repo|
|A1 Data Curation.IPYNB|Jupyter Notebook containing code and steps to execute this project.|
|pagecounts_desktop-site_200807-201607.JSON|Response data from Pagecounts for desktop through July 2016|
|pagecounts_mobile-site_200807-201607.JSON|Response data from Pagecounts for mobile through July 2016|
|pageviews_desktop_200807-201809.JSON|Response data from Pageviews for desktop through Sep 2018|
|pageviews_mobile-app_200807-201809.JSON|Response data from Pageviews for mobile app through Sep 2018|
|pageviews_mobile-web_200807-201809.JSON|Response data from Pageviews for mobile web through Sep 2018|
|en-wikipedia_traffic_200712-201809.CSV|Final output combined data used for plotting|
|en-wikipedia_traffic_200712-201809.PNG|Final output plot|

### Data Dictionary
The schema of en-wikipedia_traffic_200712-2018.CSV is:

| Column        				| Value 		|
|-------------------------------|---------------|
| year 						| YYYY	|
| month						| MM	|
| pagecount_all_views		| num_views 	|
| pagecount_desktop_views	| num_views		|
| pagecount_mobile_views	| num_views 	|
| pageview_all_views		| num_views 	|
| pageview_desktop_views	| num_views 	|
| pageview_mobile_views		| num_views		|



## Additional information

To reproduce and expand upon this work:

1. Git clone this repo
2. Run A1 Data Curation.IPYNB as a Python Jupyter Notebook.

Note that pagecount, the original traffic API, included hits from web crawlers and other automated traffic. The new Pageview API should exclude such hits.

