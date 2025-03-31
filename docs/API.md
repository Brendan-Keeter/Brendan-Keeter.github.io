## Message Comunication

### Message ID's

Name        |  ID     
------------|--------
Brendan     | B
Zack        | Z
Sivanee     | S
Carter      | C
Broadcast   | X

### Messages sent

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | Status_Wifi   | Wave_freq     | Active_status
Variable Type | uint8_t       | uint8_t       | uint8_t           
Min Value     | 0             | 0             | 0            
Max Value     | 1             | 256           | 1            
Example       | 1             | 179           | 1            



### Message Recieved

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | Tuning        | Wave_Freq     | Wave_Length
Variable Type | int           | uint8_t       | uint8_t           
Min Value     | -10           | 0             | 1 m            
Max Value     | 10            | 256           | 4.1 m            
Example       | -3            | 234           | 3 m            


### Team Messages 

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | motor_speed   | pitch_info    | Button_input
Variable Type | uint8_t       | uint8_t       | uint8_t           
Min Value     | 0 rpm         | 0             | 0            
Max Value     | 14 rpm        | 1             | 3            
Example       | 4 rpm         | 0             | 1            
