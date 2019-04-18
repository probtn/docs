 
.. _statistics_api:

Using API to get statistics data
===========

Statistics API could give you opportunity to integrate you system with admin.viewst.com 

GET-параметры запроса
----------------------------------

Params:

  * AuthKey - authorize key, give access to campaigns. This param is required.
  * AppName - apps names list for additional filtering.
  * AdSet - list of campaigns IDs, possible to find in admin.viewst.com. 
  * DateStart - date in format YYYY-MM-DD
  * DateEnd - date in format YYYY-MM-DD

Response 
----------------------------------

In response you can get requested data in JSON format.

Description:

  * adset_id - campaign
  * bundle_id - bundle id
  * datetime - datetime in timestamp format
  * content_showed - number of button clicks
  * content_showed_duration - time of the button's visibility
  * hided - number of button closings
  * moved - number of button movements 
  * moved_duration - average time for moving a button
  * opened - button impressions

Request example
----------------------------------

http://stats.viewst.com/api_reports?AuthKey=<SOME_KEY>&AppName=jgjh.ghjg&AdSet=76786786876

