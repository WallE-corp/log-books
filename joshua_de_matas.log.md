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

## Week 15 [This is being written at start of week 17]
> At the start of week 15 i worked on both the backend and the robot. I wrote and endpoint on the backend which was to used for sending up obstacle events. Obstacle events contained an image file, filename, x, and y coordinates. The endpoint takes this information and downloads the image files temporarily onto the server and attempts to upload it to google cloud storage. 

> For the robot i wrote code for creating obstacle events. The code i wrote was only to handle event once it has occured and not to detect an event. It would create an obsacle event object and attempt to upload it to the backend. If it was unsuccessful the obstacle event would be stored locally on the robot until the next time it establishes a connection or triggers another obstacle event. This code was written on our Wall-e-networking repository as a python module. I then made a pull request to our Wall-e-raspberryPi repo and implemented the new package functionality there.

> To help with setting up the socket connections I wrote the code to connect and send commands using socketIO in the mobile app. This went quick and I made a PR for the mobile team to review. 

> Cleaned up the simulation and restructured it to be more polished. Ran some tests using the simulation to plan out our future steps in the project. Implement LiDAR sensor in the simulators to better see how we can make use of it.

## Week 16 [This is being written at start of week 17]
> After a group meeting we decided it would be best to have the backend run a socket server and have mobile and the robot connect to it as clients (instead of connecting directly to each other). I then implemented a socket server on the backend and along with functionality to let the mobile and robot socket clients register who they were (in order to forward commands correctly). This code was well tested and documented. At this time i noticed how the backend code was inconsistent. I then added an ESLint config to enforce coding style. I chose a style that was as close as possible to the existing. I made a PR documenting all the features i added.

> For mobile and wallE (the robot) I updated their socket client code slightly to ensure they register their roles on the server. For walle I also updated the tests and created new ones.

> When creating the new socket server on the backend i found it annoying have to test with the mobile app all the time to i create a small c# tool that inpersonate the mobile to send commands to the socket server for manual testing. This tool can also be used much more easily by those mainly working on walle so they dont have to set up mobile environment all the time.

## Week 17
> I ended up being in charge of the backend team and lead a meeting on monday outlining which functions needed to be created. I tasked everyone with a single function to write that will then be put together to finish an entire feature. This feature was to handle obstacle events. As I had started with this a while back i had a good understanding of what was needed. My own task for the week was to clean up the backend code a bit and alter the way firebase was being used as a dependency on the backend (so that we can use better dependency injection and test more easily). 

> During the week I helped Du Won with his task which was finishing the function to upload image files to google cloud platform. We worked together one day utilizing pair programming. We implemented the function and wrote test code for it. A PR was made.

> I unfortunately ended up at the hostpital this week on Wednesday so am not able to do much rest of the week. 
