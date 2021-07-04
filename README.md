# ard_roomHeater
This README file only explains how the project works and some things that I feel are harder to understand why I used them in that way.
The file with the code is arduinoHeaterCooler.txt
Any feedback or questions on the code is much welcome as I am a beginner.

Automating a room heating system which comprises of a heat converter and a fan, using an ArduinoUno board, a 4-Relay Shield and a one wire DS18B20 thermometer and a 5k Ohm resistor.

The "heat converter” has 4 pins, 2 analog pins and 2 digital pins and using these it makes the a "request". 
The analog pins send a 0-10V signal which is the requested speed of the fan. The fan works with 3 speeds.
I've chosen to use only the analog pins because if there is a request on the digital pins, there also must be a request for the speed of the fan. 

The fan has a water system running in front of it and it can be redirected so it doesn't go for such a long ride if there is no request for temperature.(the purpose of relayValve)
Also the fan works in 3 speeds, depending on the analog request that is made.

