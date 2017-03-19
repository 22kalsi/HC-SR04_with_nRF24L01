# HC-SR04_with_nRF24L01
Building an Arduino-based wireless proximity sensor using dual HC-SR04 ultrasonic device and nRF24L01 radio module together
1. Needed libraries:
  a. NewPing library for HC-SR04: https://bitbucket.org/teckel12/arduino-new-ping/downloads/
  b. nRF24L01 library: https://github.com/maniacbug/RF24

2. Hardware connection: 
  a. The wiring of HC-SR04 and nRF24L01 can be looked up from the Internet. Make sure pin 9 and 10 are connected together with pin 10   connected with the nRF24L01 module on the transmitting side. It sounds weird but it works!
  b. Capacitor(s) must be mounted between 3.3V and GND for transmitter and receiver for stabling the performances of the nRF24L01 device, if something goes wrong (like no data is transmitted), it is usually casused by the battery with insufficient juice.

Script description:
  a. nRF24L01_transmitter.txt: the Arduino sketch for the transmitter in .txt file, one just need to copy and paste on an Arduino IDE;
  b. nRF24L01_receiver.txt: the Arduino sketch for receiver in .txt file.
PS: both scripts can be easily altered for making other low-energy consumption wireless devices;
