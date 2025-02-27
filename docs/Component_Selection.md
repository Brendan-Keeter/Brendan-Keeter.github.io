## Component Selection process and data sheet

### Major Components needed

1. Voltage regulator
2. LED display
3. Microcontroller


## Voltage Regulator
The voltage regulator is important to this subsystem as it limits the voltage and current into the microcontrollers to prevent spikes and drops of voltage and to improve performance of systems.

### Product 1: Texas Instruments IC REG BUCK 3.3V 1.7A 8SOIC

Pros                                                    |  Cons 
--------------------------------------------------------|----------------
High Output Amperage                                    | Lot of soldering pins
Lots of stock                                           | Very Small
Protective features for temperature and short circuits  | 
Switching Regulator                                     | 

![Diodes Incorporated voltage regulator](voltreg1.jpg)

[Link to diodes Incorporated Voltage Regulator](https://www.digikey.com/en/products/detail/texas-instruments/TPS5403DR/3671578?gclsrc=aw.ds&&utm_adgroup=Texas%20Instruments&utm_source=google&utm_medium=cpc&utm_campaign=PMax%20Shopping_Supplier_Texas%20Instruments&utm_term=&utm_content=Texas%20Instruments&utm_id=go_cmp-17816159938_adg-_ad-__dev-c_ext-_prd-3671578_sig-CjwKCAiAt4C-BhBcEiwA8Kp0CTcF9FVzJ_Ko_nwXZIhZdF_5RF-trQQ9HqssRgeHgRn9RdPct75E1RoCdaAQAvD_BwE&gad_source=1&gclid=CjwKCAiAt4C-BhBcEiwA8Kp0CTcF9FVzJ_Ko_nwXZIhZdF_5RF-trQQ9HqssRgeHgRn9RdPct75E1RoCdaAQAvD_BwE&gclsrc=aw.ds)

### Product 2: Texas Instruments IC Voltage Regulator

Pros                      |  Cons 
--------------------------|----------------
Very Cheap                | Limited Stock
Good output amperage      | Small size
                          | Linear Regulator

![alt text](VoltReg2.jpg)
[Link to Texas Instruments Voltage Regulator](https://www.digikey.com/en/products/detail/texas-instruments/TLV70245DBVT/3313487?gclsrc=aw.ds&&utm_adgroup=Texas%20Instruments&utm_source=google&utm_medium=cpc&utm_campaign=PMax%20Shopping_Supplier_Texas%20Instruments&utm_term=&utm_content=Texas%20Instruments&utm_id=go_cmp-17816159938_adg-_ad-__dev-c_ext-_prd-3313487_sig-CjwKCAiAtYy9BhBcEiwANWQQL6YN1oEZa4xfyE7WO1s_B3ArOTaa2NjwByYHu9_ywzZCVhIErApSexoC3EAQAvD_BwE&gad_source=1&gclid=CjwKCAiAtYy9BhBcEiwANWQQL6YN1oEZa4xfyE7WO1s_B3ArOTaa2NjwByYHu9_ywzZCVhIErApSexoC3EAQAvD_BwE&gclsrc=aw.ds)

### Product 3: Texas Instruments IC REG BOOST ADJ 980MA SOT23-6

Pros                      |  Cons 
--------------------------|----------------
Good size                 | Low max input Voltage
Easy soldering            | Low output Amperage
Boost switching regulator |

![alt text](vol3.jpg)
[Link to Texas Instruments LDO voltage regulator](https://www.digikey.com/en/products/detail/texas-instruments/TLV61046ADBVR/8133008)

### Product choice for Voltage regulator: Product 2
The Texas Instruments IC Voltage Regulator is the option I chose as it is both the correct size and amperage that is needed for this subsystem of the project. While the other 2 options were both good choices, product 1 was very limited in its capacity to output amperage and would be very difficult to solder based on its size. Product 3 was very good, however it had more pins than needed for this part of the project, so product 2 was perfect in both total pins and ease for soldering.

## LED Array
The LED array is important as it allows for a physical signal that the Wifi module is working and that the product is on.

### Product 1: Bivar Inc. Surface Mount LED

Pros                      |  Cons 
--------------------------|----------------
Multiple color options    | Small size
Very visible lighting     | Fragile
                          | Difficult to solder

![alt text](LED1.jpg)
[Link to Bivar Inc. LED](https://www.digikey.com/en/products/detail/bivar-inc/SM1204RGB/22671473?gQT%3D0)

### Product 2: 5050 3-Chip LED

Pros               |  Cons 
-------------------|----------------
Very Cheap         | Limited color options
Easy to solder     | Limited datasheet imformation
Fast shipping      | 

![alt text](LED2.webp)
[Link to 5050 3-Chip LED](https://www.superbrightleds.com/5050-smd-led-rgb-surface-mount-led-with-120-degree-viewing-angle-5050-smd-led?utm_campaign%3Dorganic-shopping%26utm_source%3Dgoogle%26utm_medium%3Dorganic%26utm_content%3D5050-RGB%26srsltid%3DAfmBOooJD4D2FlV9ukr4DnvELExSd1mPQ7Bp3z10UX3Wtdf2yv3rNDuDGCw%26gQT%3D0)

### Product 3: Uxcell 300ma 5W LED's

Pros           |  Cons 
---------------|----------------
Big Size       | most expensive option
Very bright    | Slow shipping
Comes in bulk  |

![alt text](LED3.webp)
[Link to Uxcell 5W LED](https://www.harfington.com/products/p-g0371e78e?currency%3DUSD%26variant%3D42123817255161%26utm_source%3Dgoogle%26utm_medium%3Dcpc%26utm_campaign%3DGoogle%2BShopping%26stkn%3Df8e35277684b%26srsltid%3DAfmBOopDPs2dY0Yu_6We4VzthXQTzpV-xCvpU5PApDJU0VGKCbteNZTKDkA%26gQT%3D0)

### Product choice for LED Array: Product 1
The Bivar Inc. Surface Mount LED was the choice made for this subsystem based on its visibility and the ability to shine in different colors other than just white. Product 2 was a good product, however it did not have a lot of datasheet information, which could've caused difficulty down the line with specifics when in use. Product 3 was well designed, however it being the most expensive and slow to ship was its downside. While a downside of the Bivar Inc. LED is its size, its brightness and ability to change colors were the key factors to making this choice.


## Microcontroller Information
### Microcontroller Used: Expressif ESP32 chip
![Picture of ESP module](ESPpic.jpg)
![Pin layout for Expressif ESP](<Screenshot (117).png>)
![Pin description for ESP](<Screenshot (118).png>)

### Role of Subsystem
For the team, this subsystems role is to allow communication inputs from Wifi and Bluetooth. By gathering these inputs, this subsystem will then send data to the other subsystems of the project to physically perform the action selected. Once the data has been processed by the other subsystems, it will once again be received by this subsystem and sent back out via Wifi to the user.

The main focus of this subsystems responsibilities are sensing, display, and communication. For my subsystem, it will be responsible for sensing a button press from a user over Wifi or Bluetooth connection. As it receives this data, it will display something onto their device to allow them to see more information about what the project will be physically demonstrating. The main importance of this subsystem is communication. As the subsystem recieves inputs from the user, it is sending and recieving data to and from the other subsystems in order to physically demonstrate whichever option the user had selected. 

### ESP Information
ESP Info                      |   Data
------------------------------|------------------
Model                         | ESP32-WROOM-32E-N4
Product page URL              | [Link](https://www.digikey.com/en/products/detail/espressif-systems/ESP32-WROOM-32E-N4/11613125)     
ESP32-S3-WROOM-1-N4 datasheet | [Link](https://www.espressif.com/sites/default/files/documentation/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf)
ESP32 S3 datasheet            | [Link](https://www.espressif.com/sites/default/files/documentation/esp32-wroom-32e_esp32-wroom-32ue_datasheet_en.pdf)
ESP32 S3 Technical Manual     | [Link](https://cdn-learn.adafruit.com/assets/assets/000/110/710/original/esp32-s3_technical_reference_manual_en.pdf?1649790877)
Vendor Link                   | [Link](https://www.digikey.com/en/products/detail/espressif-systems/ESP32-WROOM-32E-N4/11613125)
Code Examples                 | [Link](https://github.com/espressif/esp-who/blob/master/docs/en/get-started/ESP32-S3-EYE_Getting_Started_Guide.md)
External Resources            | [Link 1: Getting Started](https://docs.espressif.com/projects/esp-idf/en/stable/esp32s3/get-started/index.html#what-you-need) [Link 2: Complete Guide](https://www.nabto.com/guide-to-iot-esp-32/)
Unit Cost                     | $2.50
Supply Voltage Range          | Operating voltage is between 2.3V-3.6V. 3.3V Recommended
Absolute Max Current          | 1200 mA
Maximum GPIO Current          | 1200 mA
Supports External Interrupts? | Yes, it supports external interupts


Module         | # Available      |  Needed    | Associated Pins
---------------|------------------|------------|-----------------------
UART           |  3               | 2          | Any GPIO Pins
External SPI   |  4               | 2          | Any GPIO Pins
I2C            |  2               | 1          | Any GPIO Pins
GPIO           |  34              | 12         | Any GPIO Pins
ADC            |  2               | 0          | 18 Available Pins
LED PWM        |  16              | 2          | Any GPIO Pins
Motor PWM      |  3               | 0          | Any GPIO Pins

### Microcontroller Choice Statement
The EPS32 module that I had found is well suited for this project. The ESP32 that I have selected contains enough pins to be able to safely and effectively organize the board without crowding. Another thing about the board is the applications it is commonly used in. This ESP module is commonly used in sound recognition and audio devices which would suit well for the project we are working on that involves a microphone. The maximum current in the board is well within the parameters that we intend to keep our components under, so there is very little risk of damage to the EPS32 module and its recommended voltage is the exact same as the voltage we intended to use for our project. This microcontroller also has enough UART's for the project as multiple UART's are needed. This extra UART may be able to help with the debugging process as the code is being designed for this project.