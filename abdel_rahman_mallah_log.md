# Abdel Rahman Mallah

## Sprint 0 -- 21 Hours with the lectures

### 2022-03-28, Monday.

Had a meeting with the group there we talked about the project, and about the teams. We have 3 sub teams in the group. One working on the Mower (WallE), one on the UX (and Android), the last one on the Backend. I'm going to work on the backend, but of course if any subteam needs help, all the members will try to help. In this day we desided to work Agile, and voted for a Product Owner and a Scrum Master.


### 2022-03-30, Wednesday ; 2022-03-31, Thursday.

We created a Github Organization, there we are going to have, repository for each team. We created the backend repository , and the
on thursday setted up the project and installed the neccerary packages like, express for Node Js, etc. 

---

## Sprint 1 -- 23 Hours with the lectures

### 2022-04-04, Monday. 

The day started with a meeting with the group. during the meeting we talked about the what we did last week, and what each team will do this week. Then Me and the backend team started to work on the database choose, and we chosed firebase database.  We created a firebase database and connected it to the project.

### 2022-04-05, Tuesday. 

Me and the backend developers, worked on the connection with the Firebase, then the whole backend team spoke about the structure of the firebase database. After Than Ahmad And I Worked Furthur on the firebase connection and inputed mockup data to test the connection and the endPoint function.



### 2022-04-06, Wednesday. 
The day started with a mid sprint meeting , In the meeting we spoke about what each team did, what we have to do in the sprint.
    **Note:** We have 3 teams (Backend team, Mobile team And Wall-E team).Each team has a own github repository but all the repositories are in the same organization.
We spoke more about how the database should be stucture and what we need to store in the database. 

### 2022-04-07 Thursday. 

The day started with a daily meeting for 15 minutes, After the meeting I worked on a function that gets all the points from the database, then I created a pull request to merge my getAllPoints branch the main branch. 
    **Note:** Each feature we want to implements, we firstly create a branch for it then implement it, and then merge to the main.

---

## Sprint2 -- 20 Hours with lectures

### 2022-04-11 Monday. 

The day started with long meeting, where we decided the tasks for the sprint, and also decided that all the team developers should at lest be on the thursday meeting, but other meetings in the week, it is enough for just one member of each team to be on the meeting.
In the Meeting we discussed again the firebase structure and the data we need to store in the database, and made some changes to it. So the Database contains a collectoins of maps, each map contains of three lists:
    1. PathPoints
        - It is a list that contains points of the path that the Mower took.
    2. BorderPoints
        - It is a list that contains points of the map border.
    3. ObsitclesPoints
        - It is a list that contains points of all the obsticles that were found by the Mower in the map.

The tasks that we the backend team have to do those Taskes: 
    1. Fix Endpoint and run the project on Azure Server instead of localhost.
    2. AddMap.
    3. inplement getAllMaps.
    4. inplement getPathPoints.

### 2022-04-12 Tuesday

The Day Started with a meeting with the backend team developers. 
Each one of the developers took a task. I worked again on the getPathPoints which I also worked on the last sprint, I worked on it because it needed some changes after the firebase structure has changed
I also worked on getAllMaps.

### 2022-04-13 Wednesday

The day started as usual with a daily meeting with backend team developers. After the meeting I created a pull request to my branch that worked on yesterday and ask Ahmad to review it. 
Then I sat with Lucas and explained the new architecture that we are going to follow, because he was sick on that day.  

### 2022-04-14 Thursday

The day started with a daily meeting with the product owner of the project Victor, We talked about what the backend team did funtil today.

### 2022-04-15 Friday

I worked on implementing the getAllBorderPoints, and addBorderPoint functions.

---
<span style="color:RED"> <b> From now on I will either work from home or from Ahmads laptop because my laptop is not working anymore, you will find me as a coauthor in many of Ahmads commits</b></span>.

## Sprint3 -- 22 Hours with lectures

### 2022-04-19 Tuesday

The day as usual started with a meeting with the group. We discussed what we did last week, and what is needed to be done on this week. I had to delete the functions that I implemented on Friday because the group though it's not needed in the project to collect the map border.


### 2022-04-20 Wednesday

I did not work on the project my self, by I talked little bit with Duwon about the server that we need, I explained what we actually need. Because there was a missunderstanding. 
Duwon worked on creating API Server on Azure which we don't need, what we need is a server to run ours Project (API) on. Then Joshua and Duwon worked on AWS server.


### 2022-04-21 Thursday

The day started with a meeing with the group. Then I worked on fixing a bug issue that was in my previous code that Joshua noticed and created an issue on github.I fixed the bug and merged it to main. 
Then I worked on creating mockup data (path) to the mobile team, so they can try to show the path on the mobile application. 


### 2022-04-22 Friday

The day started with a meeting with the group, where we talked about what we have worked with under this sprint and started to plan to the next sprint. 
I will work with getting the lastPointId from the firebase and manage the addPoint function.

---

## Sprint4 -- 22 Hours

### 2022-04-25 Monday

Today I worked on the function managePoint, where I had to getTheLastAdded Point and add it to new point coordinates{x, y}. So when the mobile team read the points from the database they will be able to show the right point coodinates on the map.

### 2022-04-26 Tuesday

I still working on the function managePoint. What I did was to read all the points that we have in a map and save the last added point and add its coordinates to the new point, before saving it again in the database. 

### 2022-04-27 Wednesday

Today Ahmad and Me Had a long dicussion about if I did it in the right way. Ahmad had another Idea to implement the function, his Idea was to save the lastPoint in a JSON file, before we add it to the database, so when we want to add a new point we read the data from file instead of reading it from database. I though that his idea was better implementation because if we have a lot of data (points) in the database it will take few milliseconds to get the response. But by saving it in a JSON file we can secure that get the data in a faster way.

### 2022-04-28 Thursday

I worked again on the function (managePoint) and reimplemented it. Now it save the first ever created point to the file, and then whener we want to add a new point, we read the last added point coordinates from the JSON file and add them to the new added point. Then we write over the new added point to the file, so it can be used in the same way when we create/add a new point.


### 2022-04-29 Friday

The day started with a meeting with the group, where we talked about what we have worked with under this sprint and started to plan to the next sprint. 
I did not have a specifiq task to do under this sprint.

--- 
## Sprint5 -- 20 Hours

### 2022-05-03 Tuesday

At the start of the day, I did not know what I have to do because we in the backend  team was already done with all the requirements, So I talked with Ahmad and Joshua, and we decided to start to work on an extra functionalty that allow us to a new map to the database, I will in this sprint work on the implementing the map router in the presntation_layer and the map manager in the business_logic_layer. I will implement the **createMap()** function in both layers while Ahmad will implement the function in the data_access_layer.  

### 2022-05-04 Wednesday

I started to implement the createMap function in the presentation_layer (the router). I started the work on the business_logic_layer. I tested the router sending a request through Postman (Progam that allow us to send requests to the API).

### 2022-05-05 Thursday

I worked on the business_logic_layer part, where I implemented the createMap function in the mapManager. The mapManager had only one function that We implemented on the start of the project which was **getAllMap()** function. As I mentioned earlier I worked on **createMap()** function and also started to  implement a function called **getNumberFromMapId()**. The function uses another function that I later on will implement that will be called **getLastMapId()**.  

### 2022-05-06 Friday

We had a meeting were we talked about what we have done in this sprint, and what we will do in the next sprint. I will keep working on **createMap()** function in the business_logic_layer. 

---

## Sprint6 -- 20 Hours

### 2022-05-09 Monday

I worked on **createMap()** function and finished the implemention of  **getNumberFromMapId(filePath)** function that I'm using the **createMap()** function.
- *getNumberFromMapId(filePath)* &rarr; The function reads the Id from the **getLastMapId(filePath)** function (Not implemented yet) and then split the Id, and returns only the number of the Id e.g if the Id is **map_0** the function returns the number **0**.

### 2022_05_10 Tuesday

I worked on **createMap()** and finished the implemention of **getLastMapId(filePath)** function that I used in **getNumberFromMapId(filePath)** function. 
- *getLastMapId(filePath)* &rarr; The function read the last map id that is saved in a JSON file. The Id should be like **map_0**. If there is no map, the code will create a map with Id **map_1** as a Default name for the first ever created map. The function take the filePath as parameter which is the path to the JSON file that it will read from.

### 2022-05-11 Wednesday

I made some changes to the code, and moved the function **getLastMapId(filePath)** from the mapManager to the mapRepository to have a cleaner code. 


### 2022-05-13 Friday

The meeting has been canceled, but each one of us wrote what he/she did in our discord server that we use to communicate.

---

## Sprint7 -- 24 Hours

### 2022-05-16 Monday

The day started with a meeting with the backend team, where we talked abou what we have left to do. We also noticed that we had a bug in the routers. The mower team could not communicate with the database, which means that the API is not working as it should. We discussed about it and I  tried to fix it directly because it was me that worked on adding a point to the database. I did not manage to find he bug, so I will try to fix it on tuesday.

### 2022-05-17 Tuesday

I worked on the bug, Sadly after more that 3 hours I could not find the bug  in the code. So I will continue working on wednesday.

### 2022-05-18 Wednesday

Finally after 2 hours I could find the bug, and fixed it. There was no error, but there was a member that made some changes to my code and added other functions. I needed to make some reimplement router in map_router for adding a new point. Me and Ahmad have also fixed the routers, there was routers that we are using that the other member did forget to register in the awilix container when he changed the code. 

### 2022-05-19 Thursday

Today was a testing day, where we firstly updated the server with the version of the code, and then test everything with the mower and mobile teams. There was some functionalities that did not work as expected so the teams worked on fixing the bugs. 

### 2022-05-20 Friday

Today we continued on testing the functionalities. While some members are testing others started to write the required technical aspects. 
When the testing was done, we started to film the mower and record the mobile screen to use them in the presentation. 

I will also do some editing the videos and put them together. 
 








