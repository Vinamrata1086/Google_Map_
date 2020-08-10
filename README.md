# Google_Map_
Google Map 

This is android based appliction.
Look through the map and find yoruself wherever u are in the world.
This Google Map App will allow u to access your current location and to see the whole world.

The steps for creating Google-Map app are as below:

1. Creating the  Project in Android Studio
To get started, we need to create an Android project and select Google maps activity.

2.Steps for getting the Google Map API key:
Step 1: Copy the URL from the google_map_api.xml file to generate a Google map API key.
Step 2: When we paste the URL in the browser, it will open the page. Then click CONTINUE => Create API  key. The API Key will be generated.
Step 3: Copy this API key to the <string> element in the google_maps_api.xml file

3.We need to modify AndroidManifest.xml file by adding some user permission like:
1)INTERNET: To determine if we are connected to the internet or not.
2)ACCESS_FINE_LOCATION: To determine a user’s location using GPS.
3)ACCESS_COARSE_LOCATION: To determine user”s location using Wi-Fi and mobile data.

4.We will implement the android MapView in a Fragment and subsequently add the Fragment to the MainActivity class.

5.MapsActivity.java
 In MapsActivity.java class to get the Google map object, we need to implement the OnMapReadyCallback interface and override the onMapReady() callback method, these are called     when the map is ready to be used.

 Changing the Map Type: There are four different types of map Normal, Hybrid, Satellite, and terrain. We can use them as below:
 MAP_TYPE_NORMAL : The map includes a road map with street names and labels.

 MAP_TYPE_SATELLITE: This type of map has a Satellite View without street names and labels.

 MAP_TYPE_TERRAIN: The map includes colors, lines, and labels. Some roads and labels are also visible.

 MAP_TYPE_HYBRID : This map type is the combination of a satellite View Area and Normal mode displaying satellite images of an area with all labels.
 
 Add Marker on Map: We can place a marker to display location on the map by addMarker() method.
 
 In the app build.gradle file, we will add a Map dependency libraries.


Change the MAP_TYPE and see the different types of map.
