
# Smart Bin
<img src="Docs of photosd and videos/smart bin photo.jpeg">

<img src="Docs of photosd and videos/Xmas version special edition.PNG" alt="The final bin">



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

<h1>Building</h1>
<h2>Used components and tools</h2>
Reference to the datasheet in the reference list.

1. Arduino UNO 
2. Servo Motor SG-90
3. NeoPixel Stick - 8 x 5050 RGB LED
4. 2 Ultrasonic Ranging Module HC - SR04
5. Wago
<img src="Docs of photosd and videos/4 Wago Small.jpeg">
7. Jumpers (all types)
<img src="Docs of photosd and videos/electronic-jumper-wire-makers-collection-260nw-1098082193 Small.jpeg">
8. Female headers (for the LED) 
<img src="Docs of photosd and videos/female header .png">

<h3>Step By Step Instructions</h3>

1. Soldering the female header to the LED Neopixel strip
<img src="Docs of photosd and videos/LED with female header.PNG">
Connecting the LED Neopixel strip to the Arduino using jumpers
Once the female header has been attached, take the jumpers and insert them into the female header pins.
Connect the other end of the jumpers to pin 6 on the Arduino.

2. Connecting the servo
Take the servo and locate the three wires (power, ground, and signal).
Connect the power wire to the 5V pin on the Arduino.
Connect the ground wire to the GND pin on the Arduino.
Connect the signal wire to pin 9 on the Arduino.

3. Connecting the ultrasonic sensors
Take the ultrasonic sensors and locate the four wires (power, ground, trigger, and echo).
Connect the power wire of the first sensor to the 5V pin on the Arduino.
Connect the ground wire of the first sensor to the GND pin on the Arduino.
Connect the trigger pin of the first sensor to pin 2 on the Arduino.
Connect the echo pin of the first sensor to pin 3 on the Arduino.
Connect the trigger pin of the second sensor to pin 8 on the Arduino.
Connect the echo pin of the second sensor to pin 7 on the Arduino.

It is also important to note that in the code you should define the trigPin1 and trigPin2 and echoPin1 and echoPin2 as you mentioned, so that the microcontroller knows which pin the sensor is connected to.



*Please note that due to a lack of GND and 5V pins on the Arduino, a Wago connector was used to close the circuit and supply power to the components. Connect the power wire of the ultrasonic sensors and the LED Neopixel strip to the Wago connector that's connected to the 5V pin and the ground wire to the Wago connector that's connected to the GND pin. This allows for a more compact and efficient setup.

<img src="Docs of photosd and videos/1 On the Breadboard.PNG">

The photo above shows the system connected and ready for testing before deployment. All components are connected and powered as described in the instructions, double checking the connections and uploading the code to the microcontroller.


<img src="Docs of photosd and videos/3 Ultra and Wego.PNG"> 

The photo above shows the inside of the bin before it has been wrapped. The circuit board and components, including the LED Neopixel strip, ultrasonic sensors, and servo, are clearly visible. The jumpers have been organized in a tidy manner, to ensure a stable and secure connection between the circuit board and the components.  Additionally, a clipboard is used to cover and protect the wires, making the system more astatically pleasing and also protecting them from any external damage.

# Arcitecture 

 <img src="Docs of photosd and videos/Architecture.png">


# video demonstrations

# Enclosure Deployment
On the breadboard everything working fast and the sensor function and flow is perfect. 

However when I start to deploy the sensors on the box the servo cant lift the bin cover with the ultrasonic and the LED attached to it. 




# future features
1. weight sensor for indoor institutions and offices
2. LoRa (Long Range Radio) for monitoring
3. Waterprof Enclosure
4. lighting scale with the existing light


# Reference 

1. Automatic Trash Bin - https://www.instructables.com/Automatic-Trash-Bin/ - 
2. Smart Trash Bin - https://create.arduino.cc/projecthub/4DMakers/smart-trash-bin-425536


3. Arduino UNO - <a href="https://www.arduino.cc/en/uploads/Main/Arduino_Uno_Rev3-schematic.pdf">Arduino UNO Datasheet</a>

4. Servo Motor SG-90 <a href="http://www.ee.ic.ac.uk/pcheung/teaching/DE1_EE/stores/sg90_datasheet.pdf">Servo Motor SG-90 Datasheet</a>

5. NeoPixel Stick - 8 x 5050 RGB LED <a href="https://www.adafruit.com/datasheets/WS2812B.pdf">NeoPixel Stick Datasheet</a>

6. 2 Ultrasonic Ranging Module HC - SR04 <a href="https://www.micropik.com/PDF/HCSR04.pdf">Ultrasonic Ranging Module HC-SR04 Datasheet</a>


# Additional: 
Some possible microcontrollers that could be suitable for a smart bin project include the Arduino UNO, Raspberry Pi, and ESP32. Each of these microcontrollers has its own strengths and weaknesses, so it is important to carefully consider your project requirements before making a decision.





