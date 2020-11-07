# RaspberryPi-Server-Build-Flask

<img src="https://wakatime.com/badge/github/SaadAhmedSalim/RaspberryPi-Server-Build-Flask.svg" alt="time tracker" />

Before telling anything, I have tried Adafruit_DHT so many times and there is an error called 
<b>"ImportError: cannot import name ‘Beaglebone_Black_Driver’ from ‘Adafruit_DHT’" ,</b> this gave me much pain.. and after all I searched for the solution but still couldn't find any.

But adafruit_dht module works fine..No complain!

<h4>Instead of using those module, I've simply found dht11 module.</h4>

Now, I am going to tell you what I used and why.

<h2>Requirements:</h2>
      
      - Raspberry pi-4
      
      - Intellij IDEA
      
      - Python IDE
      
      - Putty and VNC
      

<h2>Documentation:</h2>

    1. import RPi.GPIO as GPIO  #pip3 install RPi.GPIO

It is a standard interface that used to connect pi with sensor DHT11. In our cases, I connect pi 1(3.3V) to DHT11(VCC), 11(GPIO-17) to DHT11(Data) and 39 to DHT(GND).

    2. import dht11 #pip3 install dht11

I use its code for my project <a href="https://pypi.org/project/dht11/">LINK HERE</a>.
  
    3. import time #pip3 install times
    
I just need it for my infinite while loop that will continuously send me the temperature and humidity. But now I am not using it.

    4. from flask import Flask #pip3 install Flask
   
Basically, flask is a web application framework and interface that has libraries and tools to build something new. In my case, I've made a web server in Pi and with the flask interface I can see it in my laptop(I have another repository where I showed it before<a href="https://github.com/SaadAhmedSalim/Raspberry-Pi-4-Network-Connection-Issues-Fixed">Click here to see it</a>).

    5. from flask_restful import Resource,Api #pip3 install Flask-RESTful
   
I give you the link to read the documentation. It is so helpful. <a href="https://flask-restful.readthedocs.io/en/latest/">LINK HERE</a>

    
  
