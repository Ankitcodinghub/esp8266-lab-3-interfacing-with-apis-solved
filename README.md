# esp8266-lab-3-interfacing-with-apis-solved
**TO GET THIS SOLUTION VISIT:** [ESP8266 Lab 3-Interfacing with APIs Solved](https://www.ankitcodinghub.com/product/esp8266-lab-3-interfacing-with-apis-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;94537&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ESP8266 Lab 3-Interfacing with APIs Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Lab Three – Interfacing with APIs

An important concept behind many innovations and advancements is to build upon or improve what already exists. In other words, it is in your best interest to use existing systems that accomplish what you plan to build upon or use as a foundation for your own work. This not only saves you time because you can spend it elsewhere working on your own key contributions rather than reinventing something that has already been done, but it can also make your own products or innovations easier to use or interface with since they build upon existing technologies. This is especially true for IoT systems and devices; one of the primary aims for IoT products is not only to allow for a network of communication between physical devices and systems, but to also do so in convenient manner by utilizing existing and flexible infrastructures.

In this lab, we will use Google APIs to add some nifty features to our smartwatch application. An API (application programming interface) makes the primary functions and commands available to the user or developer, so that they can utilize the existing technology or functionalities that the API provides. Just as a computer screen shows the user what is available or the functionalities on that computer, an API shows the developer what features of the technology are available to use. While a user can communicate actions and commands to a computer through peripherals, like a mouse and keyboard, a developer can communicate with many APIs through HTTP, an application layer communication protocol, or through the RESTful API, which uses HTTP as its basis.

For our smartwatch application, we will be using the Google Geolocation API and the OpenWeatherMap API to track the weather in our area and the Twitter API to send tweets with our smartwatch application. To incorporate these APIs, we must do the following on our ESP8266 embedded system.

Part One: Geolocation and Weather

Useful Links:

https://developers.google.com/maps/documentation/geolocation/intro http://openweathermap.org/current http://docs.micropython.org/en/latest/esp8266/esp8266/tutorial/network_basics.html http://docs.micropython.org/en/latest/esp8266/esp8266/tutorial/network_tcp.html http://www.json.org/JSONRequest.html https://developer.atlassian.com/display/CROWDDEV/JSON+Requests+and+Respon ses

http://silex.sensiolabs.org/doc/cookbook/json_request_body.html

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
1. Use an existing or create a Google account and login to the Google API developer’s console at https://console.developers.google.com/. Enable the Geolocation API and create an API key. Now that you have the API key, you can interface with the API through the ESP8266 through HTTP POST commands to the host address, https://www.googleapis.com, and by formatting your commands in JSON. This can be accomplished on the ESP8266 through the use of sockets. More information on how to setup the Google APIs are shown below.

After logging into the developers console, create a new project for your smartwatch with whatever name that comes to mind, as shown above. Once you have created your project search for the Google Geolocation API in the search bar. Once you have found the API, click the “Enable” button to enable the API, as shown below.

After enabling the API, go to “Credentials” on the left side of the screen and create an “API key”. Now that you have created an API key for the Geolocation API, you can now use Google Geolocationing in your own projects. More information on how to interface with the Geolocation API can be found here: https://developers.google.com/maps/documentation/geolocation/intro. You can find documentation about any of Google’s other APIs by looking them up on a search engine.

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
2. Now that the Google Geolocationing API has been set up on the developer’s console, display the coordinates you receive on the OLED display.

3. Feed the coordinates from the geolocation API into the OpenWeatherMap API to receive weather data for your location. Display the current weather on the OLED display. You should at least display the temperature and description (e.g. mostly cloudy). More information about the OpenWeather API can be found at http://openweathermap.org/api and http://openweathermap.org/current.

Part Two: Twitter

Useful Links:

https://apps.twitter.com/ https://thingspeak.com/apps https://ifttt.com/twitter

Interface with the Twitter API to send tweets from your ESP8266. Make sure to register for a Twitter account if you don’t have one and go to https://apps.twitter.com/ to get started. As a side note: there are many other APIs that allow you to send twitter messages, other than the Twitter API; you are welcome to use any of

them. The tweets you send do not have to be typed out and can be preset. There are links to a few other APIs listed above (Thingspeak and IFTTT) in the “Useful Links” section, that also support Twitter commands.

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
EECS 4764 Lab Three Checkpoints:

1. Interface with the Google Geolocation API and display your coordinates on the OLED display.

2. Feed your coordinates into the OpenWeatherMap API to receive information about the weather in your area; display the results on your OLED display.

3. Create a system to send tweets using the ESP8266.

</div>
</div>
</div>
