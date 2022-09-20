# Gesture-Controlled-Robotic-Arm-Wireless
This version is the advance Version of Gesture Controlled Robotic Arm Wired

The Basic of Robotic Arm will be covered at the previous model.

**_Visit_** https://muditkatiyar.github.io/Gesture-Controlled-Robotic-Arm-Wired/

**Addition of New Module**

## Nrf Module 24L01
![image](https://user-images.githubusercontent.com/113198082/191369738-ff1189ba-a986-4442-9c1f-7f46bae60c57.png)



This can be used to transmit the data of MPU6050 and Flex sensor which is fitted in the Gloves to the Module which is on the wooden board. This module is connected to the Arduino at 3.3v source which draws a current about 12 mA during transmission. The module operates on the ISM band (Industrial Scientific and Medical band) which is mostly used by the lower power device for the unlicensed user. The operating Frequency is about 2.4 GHz. The module will communicate with the Arduino in the SPI interface. This have an advantage of transmitting the data with any limit in the data which has to be transferred. The configuration in which they are connected is like a Master-Slave Configuration.
**Major Feature** -Power Efficient 

The module operates in Radio Frequency range. Transmission of data requires the channel b/w the two module. This channel is in range of about 2400- 2525 MHz , which mean that it have about 125 channel to communicate. In this project we have used 250 Kbps for uploading the data onto the channel. This information has bandwidth less than 1 MHz which make the air data rate 1 Mbps. It can use multiple module for transmitting and a single receiver. The protocol used by it as follows

![image](https://user-images.githubusercontent.com/113198082/191370454-7d9c7ad4-7cb7-4345-a012-ae3eb8a48a05.png)
Enhanced Shock burst Protocol
•	Preamble will determine the introduction of the protocol.
•	Address will determine to which address the data is sent to.
•	Packet length will determine and vary the length of the packet between 1-32 byte.
•	Packet ID will give individual id to each packet for differentiation.
•	NO Acknowledgement will be used for acknowledgement purpose to the transmitter to know whether the receiver received the packet or not.
•	Payload is the actual information transmitted.
•	CRC is Cyclic Redundancy check for determine the error in the information.

**Summary**
Operating Voltage-3.6V

Operating Current-13 mA

Standby Current-26 uA

Communication Range-800 m

Frequency Range-2.4 GHz

Modulation Format-GFSK

Interfacing With Arduino

![image](https://user-images.githubusercontent.com/113198082/191370725-40c60510-410d-4257-8997-10b7221d0a40.png)

# New Version Project Design


![image](https://user-images.githubusercontent.com/113198082/191370941-fe763903-fd29-461c-8b64-fac94635856c.png)

This Robotic Arm structure consist of  3 - MG 995 servo motor which can be controlled with the help of  3 – Flex sensor. These Flex Sensor must be fiited on the gloves. Each flex sensor must have different function to perform as follows – 
1.	Flex-1 on forefinger can be used to control the gripper motor to grip the object.
2.	Flex-2 on the middle finger can be used to control the upward / downward motion of the Robotic Arm with servo motor.
3.	Flex-3 on the Ring fingure can be used to contol the Left / Right motion of the body of the Robotic Arm.

Accuracy
The accuracy of this model is very less because while bending one flex sensor, the other flex sensor also bends which causes movement in other servo motor also. This created a problem in holding up of an object precisely. Also due to variation in the value of the flex sensor continously, the motor used to move or give a error of about 3 to 4 degree


![image](https://user-images.githubusercontent.com/113198082/191371458-c450a765-0588-4107-b7ad-071ab03f6162.png)

**Due to Low accuracy this has to be replaced with version 3**
