
# Smart Bin
#Overview
The smart bin project is an Arduino-based system that uses ultrasonic sensors and an LED to monitor and respond to the amount of waste in a bin. The first ultrasonic sensor measures the distance from the user and activates a servo to open the bin when the distance is less than 20 cm. The second ultrasonic sensor measures the amount of trash in the bin and the LED displays this information to the user by changing color. The system encourages community engagement with waste management issues and helps to optimize waste management strategies by providing real-time data about the amount of waste being generated. This project was completed as part of the university course "Making, Designing & Building Connected Sensor Systems" in 2022/2023. The project utilizes C++ programming and the Arduino IDE, as well as a variety of hardware components including ultrasonic sensors, a servo, and an LED. All components of the bin and enclosure are made from recycled materials.

This project build during the course - Making, Designing & Building Connected Sensor
Goal is to measure the 

# Libararies and define pin 
The smart bin project makes use of several libraries including Servo.h and Adafruit_NeoPixel.h . The Servo.h library is used to control the servo motor that opens and closes the bin, while the Adafruit_NeoPixel.h library is used to control the LED display. In the code, the pins for the various components are defined using #define statements. The trig pins for the ultrasonic sensors are defined as trigPin1 and trigPin2 , while the echo pins are defined as echoPin1 and echoPin2 . The pin for the servo is defined as myservo , and the pin for the LED display is defined as PIN . A list of the pins used in the project is as follows:

The main component is Arduino uno as a microcontroler that have 14 digital pins.
For this project I use 6 digital pin 

The pins: 
+ A. servo which is pin 9
+ B. define trigPin2 8
+ C. define echoPin2 7
+ D. #define trigPin1 2
+ E. #define echoPin1 3
+ F. the last pin is for the LED neo Pixel pin 6

The Libararies : 
1. Servo.h
2. Adafruit_NeoPixel.h

# Used components and tools
Reference to the datasheet in the reference list.

1. Arduino UNO 
2. Servo Motor SG-90
3. NeoPixel Stick - 8 x 5050 RGB LED
4. 2 Ultrasonic Ranging Module HC - SR04




# Arcitecture 
 ![arcitecture](Docs of photosd and videos/Architecture.png)


# video demonstrations

# Enclosure Deployment
On the breadboard everything working fast and the sensor function and flow is perfect. 

However when I start to deploy the sensors on the box the servo cant lift the bin cover with the ultrasonic and the LED attached to it. 




# future features
1. weight sensor for indoor institutions and offices
2. Add Nodemcu ESP 8266 
3. Waterprof Enclosure
4. lighting scale


# Reference 

Automatic Trash Bin - https://www.instructables.com/Automatic-Trash-Bin/ - 
Smart Trash Bin - https://create.arduino.cc/projecthub/4DMakers/smart-trash-bin-425536

Used components and tools
Arduino UNO - <a href="https://www.arduino.cc/en/uploads/Main/Arduino_Uno_Rev3-schematic.pdf">Arduino UNO Datasheet</a>

Servo Motor SG-90
NeoPixel Stick - 8 x 5050 RGB LED
2 Ultrasonic Ranging Module HC - SR04



