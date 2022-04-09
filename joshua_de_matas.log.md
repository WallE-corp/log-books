# Joshua De Matas work log
For Intelligent Mobile System

## Week 13 - Project Start 
### Monday
#### What we did
>First group meeting. Mainly led by me. We did a rough introduction of our selves and what we'd imagine us to work on. Decided discord will be our tool of communicaiton.
#### What I did
>Gathered everyone's discord handles then created and invited everyone to a discord server specifically for the project.

### Wednesday
#### What we did
>Had a long meeting to get the project of its feet. Walked through as a group and broke down the high level requirements given to us. Also began our Work Breakdown Structure. Decided on who will work on what and generally how.
#### What I did
>Started working on a simulation for the robot.
### Thursday
#### What we did
>Met during the lab session. I was late. Not official meeting. Mianly talked in smaller conversations as we were begining on our own parts.
#### What I did
>Mainly assisted the others with starting up their github repositories. Also created a Github organization and invited everyone.
>Continued to work on the simulation. Implemented a variation of the Marching Squares algorithm and the Digital Differential Analyzer algoirthm (Super proud of these two :3).
<details><summary>Reflections</summary>
The initial week felt good. I unfortunately missed the first part of the lab session on Thursday which really isn't good to set the tone of the whole project.
</details>


## Week 14 - Making sure everything is connected
#### What we did
>I missed monday's meeting due to health issues. The group was appointed a new leader (was initially me). A new scrum leader was also appointed (previously Lucas)
#### What I did
>Wrote code for running a socket server in C which was meant to be used for the robot. However, the robot team decided on using Python to handle communication with the other components. So I initially created a quick socket server in Python and tested it along with the guy working on the robot. We were able to control and steer the robot by sending commands from a client to the server. After this proof of concept I revised the code for the socket connection so that it is well tested, easy to implement, and documented. Starting on python module to be used for connecting to the back end. 