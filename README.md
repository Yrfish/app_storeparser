# app_storeparser
AppStore parser looking for kind of data about app 

I have a list of AppStore apps urls in xlsx sheet

↓↓↓↓↓↓↓↓ below acrions in loop for each app ↓↓↓↓↓↓↓↓ 

Collect those urls to list and go trought for loop.  
Go to app urls to collect basic data that i need: subscription, descripeion, rating, language, privacy url, developer url. 
 Than go to privacy url with Selenium to search email. For thar i use re expression. Use Selenium bacause some sites has email protection After all write data to xlsx and save it every 30 iteration and save it if eroor caused

Script has check for response 404 than it save xslx and write to app cell "cant connect" if response 429 - wait for 30 sec and try agin
