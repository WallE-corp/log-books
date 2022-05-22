# **2022-03-28**

First meeting. Settling on roles within the group.
I’m in the mower team. 

# **2022-03-30**

Planning meeting for the whole project.

# **2022-03-31**

Setting up Mblock and Arduino. Working on basic turn and navigation functions for the mbot.

# **2022-04-07**

Set up the raspberry pi camera, can now take a picture.
Implemented line follower function using the mbot sensors.
Set up socket connection with robot. 

# **2022-04-11**

Planning meeting with the whole team. How mapping out the area which the robot operate within was discussed. The robot team will send x & y coordinates to the backend and use deadreckoning to calculate positioning

# **2022-04-13**

The robot team set up the gyroscope of the mbot to get the direction of the robot. We also installed the accelerometer on the Raspberry Pi. 

# **2022-04-14** 

We calculated the velocity of the robot with RPM(revolutions per minute) and the radius of the wheels.
With the direction from the gyroscope and the calculated velocity we can use deadreckoning to calculate the positioning (x,y).

# **2022-04-15** 

Weekly planning meeting.

# **2022-04-19** 

Weekly planning meeting	

# **2022-04-21** 

Finished deadreckoning algorithm to get (x, y) coordinates. 
Worked on obstacle detection function.

# **2022-04-22**

Weekly planning session.

# **2022-04-28**

Setting up function for camera recognition function to prevent overwriting of the picture taken. 
Setting up switch statement to handle automatic and manual mode.

# **2022-04-29** 

Weekly planning meeting. Next week we try to send (x,y) coordinates + images of objects to the backend.
Bluetooth connection was also discussed, but no conclusion was drawn.

# **2022-05-04**

Tested sending position data to backend (x,y) along with a image when the robot detects an obstacle.

# **2022-05-05**

Simulated connection of mobile and the mower through a socket. Tested the different moving commands.
Switched the Raspberry Pi Zero to a Raspberry Pi 4.

# **2022-05-06**

Weekly group meeting. Discussing what was left to do in the project. 

# **2022-05-11**

The mower team worked on fixing how we send and recieve data between the Arduino and Raspberry Pi due to data being overwritten. 

# **2022-05-12**

Worked on some minor issues with basic functions.
Made sure we were ready to test next week. 

# **2022-05-19**

Made sure that backend is recieving data.

# **2022-05-20**

Meeting with the whole team to finish the project. The mower squad worked on documentation and the lessons learned documentation.
We also recorded the final video for the presentation. 

