I'm sorry, but the repository is not going to be updated.

ATTENTION! the protocol can't use.

If you want to get software, please click the offical websit.
http://dobot.cc/

Ofcourse, you can fork the repository and fit protocol to work. 

Dobot
================================================
![image](https://github.com/kidswong999/dobotArm/raw/master/doc/media/dobot_logo.png)

1.Machine Sketch
-----------------------------------------------
![image](https://github.com/kidswong999/dobotArm/raw/master/doc/media/3D_coor.png)

2 Communication Protocol
---------------------------------------------------------------------
####1 Parameters setting
Baud rate:256000.
Parity:  None.
Stop: 1.
####2 begin communicate
PC send beginPackage{}, and communicate is beginned. 
later Lower machine send data requestPackage{} per 60ms.



		beginPackage
		{
			0xa5,0x00,0x00,0x11,0x11,
			0x22,0x22,0x33,0x33,0x00,
			0x00,0x00,0x00,0x00,0x00,
			0x00,0x00,0x00,0x00,0x00,
			0x00,0x00,0x00,0x00,0x00,
			0x00,0x00,0x00,0x00,0x00,
			0x00,0x00,0x00,0x00,0x00,
			0x00,0x00,0x00,0x00,0x00,
			0x00,0x5a
		}
		requestPackage
		{0xa5...0x5a}
		38byte
####3 move control
after resceived the requestPackage{}, PC send controlPackage{}.


c
		
		code
		

c++
		
		code
		

python
		
		code
		

java
		
		code
		

c#
		
		code
		


4 Arduino software
--------------------------------------------------------------------

5 schematic and PCB board
-------------------------------------------------------------------
