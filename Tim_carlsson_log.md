## 2022-03-28, Monday.
The initial meeting with the designated project group in which each team member assumed a role within a set of sub teams aimed towards either the backend, the mobile application, or the robot which we designated as Wall-e. I alongside the other DIS students joined the wall-e team. For me personally I found the robot to be the most intriguing and fitting part for me to work. Additionally, everyone agreed that if one team “falls behind” they will receive assistance from the other teams.
## 2022-03-30, Wednesday.
During this meeting we planned the project and created the GitHub organization and most of the repositories with it. Additionally, the robot was assembled according to the land raiser specification. 
## 2022-03-31, Thursday.
The first dedicated lab session was utilized for the gathering of any and all necessary software such as Mblock which is the program for controlling the robot’s functionality. Additionally, we searched for and downloaded the Arduino IDE which allowed us to edit the code directly instead of only through blocks since Mblocks software prohibited direct changes of the code.
## 2022-04-04, Monday. 
Our primary goal was to figure out and facilitate the connection between the robot and the raspberry pi. This was achieved through a setup serial communication between the two which allowed us to send signals both from the PI to the Arduino and from the Arduino to the PI.
## 2022-04-06, Wednesday.
Testing of serial communication by sending data to and from the Raspberry PI and the robot. Also steering the robot through these signals sent by the raspberry pi.
## 2022-04-07, Thursday.
Primarily development of the robot’s functionality such as the ability to detect a line which in this context is black tape as well as the ability to follow this tape around the area. Additionally, we connected the camera with the pi and tested it out by taking pictures and saving them on the pi. Also successfully controlled the robot through a socket connection by sending movement commands.
## 2022-04-13, Wednesday.
Started looking at the means of sending positional data from the robot. We decided upon dead reckoning which requires us to use data such as velocity and direction from the robot. We tried several means of sending velocity but decided upon calculating it through the RPM produced by the motors. 
## 2022-04-14, Thursday.
We worked on sending and receiving several pieces of data at the same time. Data such as RPM and information from the gyroscope and additional checks. Furthermore, foundations for triggering the camera to take a photo from the robot.
## 2022-04-15, Friday.
We had a meeting where we discussed feedback received from the meeting with the Husqvarna representatives. Additionally, we discussed several approaches and means of implementing the handling of the positional data and any issues that pertains to it. Also laid out the plan for the coming week.
## 2002-04-21, Thursday.
Implemented the functionality for calculating once position through an inertial navigation system that was implemented via dead reckoning. This feature was moved from the PI to the Arduino  board on the robot in order to ease the load for the pi since it was becoming overloaded. Allowing us to send our x and y position relative to our last update. Additionally, setup the sending of multiple pieces of data such as the object detected in addition to position data.
## 2022-04-22, Friday.
Checkup meeting regarding next weeks steps and the structure behind the communication between the phone and robot.
