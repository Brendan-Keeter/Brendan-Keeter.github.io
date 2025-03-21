## Message Comunication



### Messages sent

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | Status_Wifi   | Wave_freq     | Active_status
Variable Type | uint8_t       | uint8_t       | uint8_t           
Min Value     | 0             | 0.0012 Hz     | 0            
Max Value     | 1             | 0.0104 Hz     | 1            
Example       | 1             | 0.0079 Hz     | 1            



### Message Recieved

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | Tuning        | Wave_Freq     | Wave_Length
Variable Type | int           | uint8_t       | uint8_t           
Min Value     | -10           | .0012 Hz      | 1 m            
Max Value     | 10            | .0104 Hz      | 4.1 m            
Example       | -3            | 0.0093 Hz     | 3 m            


### Team Messages 

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | motor_speed   | pitch_info    | Button_input
Variable Type | uint8_t       | int           | uint8_t           
Min Value     | 0 rpm         | 0             | 0            
Max Value     | 14 rpm        | 1             | 3            
Example       | 4 rpm         | 0             | 1            
