# @quiztime challenge

Date: Jul 4th 2022

Link: https://twitter.com/bayer_julia/status/1544078366990602245

(<img width="589" alt="quiztime_2022jul04" src="https://user-images.githubusercontent.com/111104710/184282660-d791fc73-5f65-415c-99d4-91ba1fd78461.png">

### The tower
Checking @bayer_julia's Twitter profile, we are lead to https://about.me/juliabayer, where we find that they are a journalist from Berlin, Germany. This is a good indiacation that the image was taken in Berlin. Searching for *tall towers berlin* via Duck Duck Go images, I found a number of matches to the quiztime image:

<img width="1368" alt="duckduckgo_tower_search" src="https://user-images.githubusercontent.com/111104710/184283195-468298a6-8b8a-4f27-89aa-6269ddeb7a3e.png">

Based on this we can tell that the tower in question is [Fernsehturm Berlin](https://en.wikipedia.org/wiki/Fernsehturm_Berlin).

### Location
I initially searched around with Google Earth to see if I could find the side and angle of where the picture was taken and see if I could track down the location that way. While I got close, this definitely was a longer process. I switched to analzying the road signs that can be seen in the picture. There is a particular one that seems to indicate some parking zone information:

<img width="353" alt="road_signs" src="https://user-images.githubusercontent.com/111104710/184283588-fe76529c-0e17-4968-9325-4fb84a200044.png">

Using a [text extractor tool](https://brandfolder.com/workbench/extract-text-from-image), I was able to obtain the text from the sign:

```
Mit Parkschein oder
Bewohnerparkausweis
für die Zone 29
Mo-Sa 17-24 Uhr
So 9-24 Uhr
```

A quick trip to Google translate:

```
With parking ticket or Resident parking permit for zone 29 Mon-Sat 5-24 pm Sun 9am-24pm
```

So we now know that this relates to Zone 29 for parking within Berlin. There are numerous websites that give us details on parking permit zones for Berlin that were useful in my research. I quickly found out that this was referring to the Mitte part of Berlin and so I focused my searches there. I will name a few sites here that provided help with maps for the parking zone:

* https://www.berlin.de/ba-mitte/politik-und-verwaltung/aemter/amt-fuer-buergerdienste/buergeraemter/artikel.244758.php
* https://www.berlin.de/ba-mitte/politik-und-verwaltung/aemter/ordnungsamt/parkraumbewirtschaftung/220316_gesamtplan_parkraumbewirtschaftung.pdf
* https://www.berlin.de/ba-mitte/politik-und-verwaltung/aemter/ordnungsamt/parkraumbewirtschaftung/ >> Within this site I was able to download PDF maps of the parking zones
* https://www.google.com/maps/d/viewer?mid=1v1FrOhbc4cXrtsVLkFY-jQSi5sc&ll=52.52705919186779%2C13.39742748925675&z=17 >> In the end this proved to be the most useful

<img width="1370" alt="Berlin_Paid_Parking_-_Google_My_Maps" src="https://user-images.githubusercontent.com/111104710/184287312-a7ae5c25-bf1f-4e0b-8838-288f7f6e4f26.png">

My main tactic was to try different streets to see if they appear familiar and if I can get the right angle and view of the tower via Google Street View. 

Eventually navigating through the streets, I located **Rosenthaler Str., Berlin, Germany** which seemed to be matching a number of characteristics. I note that I haven't seen recent Google Maps Street View updates for Berlin, the images were from July 2008 but there were several characteristics that stood out.

<img width="1378" alt="19_Rosenthaler_Strasse_-_Google_Maps" src="https://user-images.githubusercontent.com/111104710/184285273-c1c84651-b685-42a4-b27f-e0db516f772f.png">


### Solution
While the image is slightly older and the sign as well as some of the sites look to have changed, I believe the location has been found for where this image has been taken:

* 52.5268254,13.4034432
* 19 Rosenthaler Str., Berlin, Germany

<img width="1379" alt="image_comparrison" src="https://user-images.githubusercontent.com/111104710/184286722-11b6c0c7-bbd5-4750-a3d6-9354eb2f48f7.png">
