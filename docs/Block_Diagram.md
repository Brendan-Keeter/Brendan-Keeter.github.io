## Block Diagram of 2 way wifi communication


This block diagram is the MQTT communication portion of our project. The MQTT system is connected via WIFI communication with my microcontroller, the ESP32. The system included 2 different voltages on the board, a 9V which is going into both the voltage regulator and the header pins, and a 3.3V which goes directly into the ESP32. The ESP32 is connected to a USB port in able to code and an LED is being used for debugging purposes. The UART communication is taking in and sending out data from the other subsystems through pin 2 of the header pins.




![Block Diagram](1746169004370-98db2433-7757-4303-a6fa-597b9f8fed9f_1.jpg)

[Block Diagram PDF](Block_Team203_Keeter.pdf)

[Block Diagram Source](https://drive.google.com/file/d/1lBq51Aa4LJ1upC8nbrsn0R02aSWhaZRm/view?usp=sharing)

