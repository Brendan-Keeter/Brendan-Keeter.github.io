## Schematic

The goal of my schematic was to make a design that would be able to broadcast data to the user of our project. I had the MQTT subsystem, so while my schematic didn't have a lot of physical hardware, the internal hardware and code was very important. In order to broadcast MQTT, I had selected the ESP32 microcontroller for my schematic since it contains Wifi capabilities. My board was selected from the team to also be the power source for the entire team so I had selected a voltage regulator that was able to take in higher voltages, that way I could use a power source that would provide enough current to everyones systems. 

With the ESP32, I am able to connect to an MQTT Explorer that will allow me to showcase all the data that we had received. In our teams mission statement we had mentioned how we wanted to create an interactive product for k-8 students. When the students would speak into the microphone attached to another team members subsystem, the values would then be sent to me to process into a way that can be understood easily for the user. These values I'd recieve (pitch, motor speed, frequency) would then be used in the ESP32 to show the user things such as their tune(whether sharp or flat), their key, and what the vocal frequency was. These values satisfy this user need as it allows them to have an interactive experience and see how the way they speak into the microphone affects the sound wave. 

This schematic also being designed to be the power source for our entire system gave my schematic the ability to also act as the ON/OFF system for the entire product as well. Once the user was done with the product or wanted to try something else, they would be able to change the state from ON to OFF. This would cause messages to stop being passed between our boards via the daisy chain, effectly turning the microphone and motor subsystems inactive till the state was switched back from OFF to ON. 


### Schematic Design

![Schematic](1746056911005-8b6e04da-d1b4-412d-91ec-ea043bb2be19_1.jpg)


[Schematic PDF](Final_Schematic.pdf)


### Power Budget

![Power Budget](1740775855263-a0fc072d-b641-4deb-8700-291f5a488f14_1.jpg)

[Power Budget PDF](<power budget - Sheet1.pdf>)

[Power Budget Link](https://docs.google.com/spreadsheets/d/1vRoSXK202q8WlBCtyZgGOLbRly6qO8YX6i80h-ZgNSs/edit?usp=sharing)

By creating this power budget, I was able to see just how much current and voltage I would need to get my system running properly with a 25% safety cushion if every system were to run at maximum current. The one thing I found when making my power budget was that I needed a wall mount power source that had a bit more current due to the maximum current that my voltage regulator was going to need. For the power budget, when totalling the maximum current for everything with the wall mounts power, the remaining current is very close to 0 mA, however I will not be needing to run every part of my subsystem at maximum current at any time.

This schematic helps to satisfy user needs and requirement for our product as it allows for successful communication through Wifi. The schematic itself is very simple as most of the resources will be in coding, however it was important to our team that there be UART communication and LED's to communicate between each of our subsystems and also be able to shine an LED to inform the user that they are connected to the Wifi module. It helps us to meet our user needs as it allows for the user to get extra resources to learn from as an input is being recognized by our project.


### PCB Design

![PCB Top Layer](1746058921717-ecc4879e-0df6-4f3c-8703-2a990cf017c0_1.jpg)

![PCB Bottom Layer](1746058921674-9e5a4f5f-fab9-4f86-b45e-b87278dfe8bf_1.jpg)

[PCB Top Layer PDF](Final_PCB_top.pdf)

[PCB Bottom Layer PDF](Final_PCB_bottom.pdf)

### Zip file for project workspace

[Project Zip File](<Final_PCB (4-30-2025 5-21-09 PM).zip>)

[Project Gerber Files](Gerber.zip)


### Version 2.0


If I were to make a version 2 of my schematic, the first thing I would add would be more debugging ports. While debugging my board, there were multiple times that I was left unsure with what was causing a problem I had run into. If I were to add more GPIO pins and LED's, this would have allowed me to easily diagnose where a problem was occurring. An example was when I was trying to get my ESP32 to program with the communication code. I was able to create a sample code for a seperate ESP32 Devkit and wanted to test if my board was able to work without having it contsantly plugged into my PC. I only had the 1 LED attached to my board and it was having difficulties lighting up so I knew that I had an issue somewhere in my system, however since the one LED is at the end of the circuit, I was unsure of where the problem occurred.

Another problem I would've changed would be to double check the capacitors for my voltage regulator. I was able to get my voltage regulator working for my ESP32, however I had needed to add in parallel a few external, through hole capacitors to keep the voltage regulator from flucuating too much. This proved to be a problem at the beginning of the project as I had ended up burning through 2 ESP32 microcontrollers I had attached to my board. When I tested the voltage with the multimeter I had an average voltage of 3.3V, however, once I had tested with the Oscilioscope, I found that, while the average voltage was 3.3V, the range was between 2.9V and 3.7V, both of which are outside the safe operating parameters of the ESP32 module.

These improvements would've helped the project as they would've allowed for diagnosing problems earlier into development and allowed me to have avoiding needing to replace the ESP32's that I had burned up.