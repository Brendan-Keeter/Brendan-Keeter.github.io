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

### Message Type

Message Type    |  Values  | Type
----------------|----------|-----------
Motor Freq      | 1        | 0x31
Motor ON/OFF    | 3        | 0x33
System ON/OFF   | 4        | 0x34


### Values

Message Type    |  Values  | Type
----------------|----------|-----------
Motor Freq      | 0-255    | 0x30 - 0xFF
Motor ON/OFF    | 0-1      | 0x30 - 0x31
System ON/OFF   | 0-1      | 0x30 - 0x31
Sensor Error    | 0-6      | 0x30 - 0x35
Motor Error     | 0-6      | 0x30 - 0x35
MQTT Error      | 0-6      | 0x30 - 0x35

### Error Types

Error type              | Value
------------------------|-----------
Wrong start to message  | 0x30
Wrong Sender            | 0x31
Wrong Receiver          | 0x32
Wrong Message Type      | 0x33
Wrong Message Value     | 0x34
Wrong Message ending    | 0x35 

