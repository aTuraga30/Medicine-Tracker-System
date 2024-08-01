# Medicine Tracker System
The repository for all files related to the medicine tracker system project

This project was created to help our seniors remember to take their medicine on time. The idea is that when a caretaker or family member sets a time on an app, at that time, the reminder band for the senior will light up, letting them know it is time for them to take their medicine. Once they have finished taking their medicine, they can push a button on the band and the light will stop. The app will also take a note of when they took their medicine last.

There are two parts to this project: the application and the physical circuit itself. 

# The Application 

The application is where a caretaker can set the time to remind the senior at. They are able to set the time on the app, and when that time is reached, then the app will send an API Request with a value of '1'. This signifies that the user needs to take their medicine. 

<img align="left" width="300px" src="https://github.com/aTuraga30/Medicine-Tracker-System/blob/main/app%20images/app_page1.PNG?raw=true">
<img width="300px" src="https://github.com/aTuraga30/Medicine-Tracker-System/blob/main/app%20images/app_page2.PNG?raw=true"> 

## Installation 

To get started, an installation of flutter is required. Check it out at: https://docs.flutter.dev/get-started/install

Next, navigate to the project's home directory which is: /finalstemapp

Then run the following:
`flutter run`

# The Circuit 

The circuit is the representation of the band in the project. It is comprised of an ESP32 microcontroller which controls an LED. When the application send an API request of '1', the circuit will read it, and consequently turn the LED on. When the user is done taking their medicine, they simply push the button, which sends an API request of '0'. The ESP32 will read this signal and consequently turn the LED off. 

The API used in this project was provided through 'ThingSpeak'. Link to their website: https://thingspeak.com/.

# Summary

This project was the culmination of 2 years of work through Fairview High School's STEM Academy. It won multiple state-level awards through the Pennsylvania Junior Academy of Science. 
