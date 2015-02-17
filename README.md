#Unofficial Major Leauge Hacking API

Welcome to the Unoffical MLH API. This is not the offical API used by MLH, but simply one I made a CodeDay Winter 2015.
The API is a simple REST made in Flask that utilizes BeautifulSoup. The API pulls data from MLH website depending on the season you specify in the URL.
Currently `s2015` maps to the United States events and `2015-eu` to the European version. 

The app returns basic information about each event including the offical id, data, link, location, and name.  
The following example is the first element if `event/dragon%20hacks/` is selected. 

``` json
"Dragon Hacks": {
    "date": "January 10th - 11th",
    "id": "102",
    "link": "http://www.hack-dragon.com",
    "location": "Philadelphia, PA",
    "name": "Dragon Hacks"
  },
  ```
  
  You can also select individual querys of hackathons such as the `link` or `id` using the url mapping `/search/name_of_hackathon/value`. For example `search/dragon%20hacks/date` would return  
  ``` json
  January 10th - 11th
 ```
 
 or `search/dragon%20hacks/link` would return  
 ``` json
 http://www.hack-dragon.com
 ```
  
  
  Feel free to edit and manipulate the code as you like. I hope this code is as useful as I thought it would be. 
