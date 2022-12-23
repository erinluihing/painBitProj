# painBitProj

Title: PainBit Chronic Pain Tracker

Description: Arduino code being created for the painBit which is a wearable device being created to store chronic pain data. The user should be bable to callibrate ten levels of pain with a pressure sensor, which will be stored in the Arduino. Then, the PainBit will identify the level of pain anytime the user experiences chronic pain and presses the sensor. Everytime the sensor is pressed, the uesrs level of pain should be stored in the arduino's memory so that the levels of pain can be accessed later. 

Installation and Running: The code can be used with the Arduino by pressing run then uploading the code to the Arduino board through the Arduino software.


To use the project: The code is set up in segments as seen by the comments. The beginning is the libraries used, including EEPROM which is the storage used to store the pain levels. Then the screen display size is declared as well as the address of the display and the pressure sensor reading is initialized. The rest of the code intializes the use of the display and displays the Adafruit logo which is the creator of many of the code tempaltes I used. 

Then the functions to write and read from the EEPROM Arduino storage were created. Then the testpainbit function is the overall function that the code calls to display text to the user, and begin callibrating pain levels. Once callibration is ran for all ten levels and the code begins monitorinhg for pain levels, which is constantly checkign to see what number of pain is at the pressure sensor. This compares the level of pain at the sensor to the callibrated pain levels. Anytime the Arduino finds a certain pain level pressed at the pressure sensor, it writes that level of pain into the EEPROM storage to keep track of what pain levels were experienced. 

To read back the levels of pain Stored in the EEPROM, the read_eeprom code can be sued, which was taken from the Arduino library of EEPROM code examples. This simply reads all the slots of memory in EEPROM.

Before starting a new user with the PainBit, all the EEPROM memory should be cleared which can be done using the eeprom_clear code, which was also taken from the Ardunio library of EEPROM code examples.

Credits: Pieces of code were used from the below links. 
https://www.youtube.com/watch?v=RjyulqVsz2o&list=WL&index=20&t=622s 
https://www.youtube.com/watch?v=eW3SQCi0aTE&list=WL&index=24
https://www.youtube.com/watch?v=7x1P80X1V3E&list=WL&index=26 
And credits to William Dorval for code help. 
