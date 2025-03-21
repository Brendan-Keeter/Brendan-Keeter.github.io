## Message Comunication



### Messages sent

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | Status_Wifi   | motor_speed   | ETA
Variable Type | uint8_t       | ETA           | ETA           
Min Value     | 0             | ETA           | ETA            
Max Value     | 1             | ETA           | ETA            
Example       | 1             | ETA           | ETA            



### Message Recieved

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | Amplitude     | Wave_Freq     | Wave_Length
Variable Type | uint8_t       | uint8_t       | uint8_t           
Min Value     | 0 rpm         | .0012 Hz      | 1 m            
Max Value     | 14 rpm        | .0104 Hz      | 4.1 m            
Example       | 9 rpm         | 0.0093 Hz     | 3 m            


### Team Messages 

Type          | Byte 1        | Byte 2        | Byte 3         
--------------|---------------|---------------|---------------
Variable Name | motor_speed   | Status_Active | Button_input
Variable Type | uint8_t       | uint8_t       | uint8_t           
Min Value     | 0 rpm         | 0             | 0            
Max Value     | 14 rpm        | 1             | 3            
Example       | 4 rpm         | 0             | 1            
