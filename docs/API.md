## Message Comunication

In order to communicate with each other without having structure issues between the ESP32 and PIC, we decided as a team to relay all our messages in Hex form rather than binary
In our messaging, the controller will begin reading a message once it sees the values AZ((0x41)(0x5A) in Hex). The message will end when it receives the values YB ((0x59)(0x42) in Hex). The message will be at most 64 bytes long.

## Message structure

Example Message Structure: [AZ][SENDERID][RECEIVERID][MESSAGETYPE][VALUES][YB]


### Sender ID's

Name        |  ID    | Value 
------------|--------|------------
Brendan     | B      | 0x42
Zack        | Z      | 0x5A
Carter      | C      | 0x43

### Receiver ID's

Name        |  ID    | Value 
------------|--------|------------
Brendan     | B      | 0X42
Zack        | Z      | 0x5A
Carter      | C      | 0x43
Broadcast   | X      | 0x45

### Messages sent

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | Status_Wifi   | Wave_freq     | Active_status
Variable Type | uint8_t       | uint8_t       | uint8_t           
Min Value     | 0             | 0             | 0            
Max Value     | 1             | 255           | 1            
Example       | 1             | 179           | 1            



### Message Recieved

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | Tuning        | Wave_Freq     | Wave_Length
Variable Type | uint8_t       | uint8_t       | uint8_t           
Min Value     | -128          | 0             | 0 m            
Max Value     | 127           | 255           | 255 m            
Example       | -3            | 234           | 47 m            


### Team Messages 

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | motor_speed   | pitch_info    | Button_input
Variable Type | uint8_t       | uint8_t       | uint8_t           
Min Value     | 0 rpm         | 0             | 0            
Max Value     | 255 rpm       | 1             | 3            
Example       | 4 rpm         | 0             | 1            
