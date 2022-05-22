# Ahmad Abdullahs log-book

in this course i worked at average 20 hours including meetings and lectures associated with the course.
# Week 13
## 2022-03-28, Monday.

 
We had a meeting with the team to start organizing the project, to determine which team everyone might want to be on, and break it into tribes based on people's interests.
 I joined the backend team or the mobile team if we are working with native languages since I have worked with cross-platform frameworks for a long time. 
 However, we have determined that everyone would be flexible and support each other as needed.

 
---
## 2022-03-30, Wednesday 


 

Me and abed sat reading bout swaggerhub for the sake of testing and documenting the project on the go.

 
---
# Week 14
## 2022-04-04, Monday

 
Since our product owner could not attend to the meeting he asked me to stand up instead of him in this day as a product owner. 
Since i did not had the time to create product backlogs and  i tried to figure out what to do on the go, 
We started with a project group meeting where we discussed what we did the previous week and what we want to do this week, and the backend team decided to adopt Firebase as a database.

 
---

## 2022-04-05, Tuesday.
 
We had a meeting with the rest of the backend developers,
 and we built the connection to Firebase, spoke about how our firestore structure would look, 
 and Abdel and I worked on the firebase further so that we could read and write data in the database. 
 Finally, we established a connection between our API and Firebase.
 
---

## 2022-04-06, Wednesday
 
We held a mid sprint meeting to make it clearer on what we should work on. 
Because until this day we did not know how to function as a team. Since our product owner did not create a user story backlog i created our backlog based on what we planned to do in the original sprint meeting and based on the product itself. it made it much more clearer for the rest of the group and we could create more functionalities as a team. I took the getPointById endpoint. 

 
---

## 2022-04-07, Thursday
 
 we held a normal standup meeting to  review what we did and how much time we had left on what we started with, and we made a few adjustments to the database structure, and the function was eventually completed later that day. and i made a pull request to the main brach and still waiting for my code to be reviewed and accepted by my fellow team mates to merge it into the main brach, i requested Abdel and do won.

 
---



## 2022-04-11 Monday. 

 
The day began with a lengthy meeting in which we determined the sprint's tasks and resolved that all team developers should attend the Thursday meeting at the very least, but that subsequent meetings during the week can be attended by simply one member of each team.
We discussed the firebase structure and the data we need to put in the database again in the meeting, and made some improvements. As a result, the Database comprises a collection of maps, each of which has three lists:
1. PathPoints
     * It's a list of points along the course taken by the Mower.
2. BorderPoints
     * This is a list that includes map boundary points.
3. ObsitclesPoints
     * It's a list that includes the locations of all the obsticles discovered by the Mower on the map.

The duties that we, the backend team, must do are as follows:
1. Replace localhost with Azure Server and run the project there.
2. AddMap.
3. Add in getAllMaps.
4. Activate getPathPoints.
 
---

## 2022-04-12 Tuesday
 
The day began with a meeting with the backend development team.
Each developer was assigned a task. I worked on documentation and swagger code and some code test setup, because it needed some tweaks after the new endpoints we decided firebase structure changed.
I also contributed to the code review for the other team members.
 
---

## 2022-04-13, Wednesday
Abdel = Abdelrahman
 
The day started as usual with a daily meeting with backend team developers. 
After the meeting i reviewed Abdels code which was very good.

Because Lucas was sick that day, I and Abdel sat with him and outlined the new architecture we'd be following. 
 
---


## 2022-04-14 Thursday

 

The day began with a daily meeting with the project's scrum master, 
Victor, during which we discussed the backend team's activities up to this point.
 
---

## 2022-04-15 Friday

i worked on updating some functionality with Abdel.
 we have updated the get all path points funtionality.  

---


## 2022-04-19 Tuesday

The day began with a group meeting, as is customary.
We spoke about what we did last week and what we need to do this week.
I had to remove some functionalities I built on Friday because the group decided that 
collecting the map boundary was unnecessary for the project.

---

## 2022-04-21 Thursday
 
A group meeting kicked off the day. Abdelrahman discovered a weakness in my previous code and reported an issue on github. The fix was merged into main.
Then I developed path mockup data for the mobile team to display in the app.
 
---

## 2022-04-22 Friday

 
The day started with a group meeting in which we discussed what we had accomplished throughout the sprint and started planning for the next one.
I'll be in charge of getting the lastPointId with abdel from Firebase and administering the addPoint method.
 
---

## 2022-04-25 Monday

 
Today I worked on the function managePoint, where I had to getTheLastAdded Point and add it to new point coordinates{x, y}. So when the mobile team read the points from the database they will be able to show the right point coodinates on the map.
 
---

## 2022-04-26 Tuesday
 
I started to work on get image classification, 
so first of all i needed to decide which classification service is best. it was a bit hard to choose between the diffrent services since every one had its ups and down
 
---
## 2022-04-27 Wednesday
 
Today Ahmed and Me Had a long dicussion about if I did it in the right way. Ahmed had another Idea to implement the function, His Idea was to save the lastPoint in a JSON file, before we add it to the database, so when we want to add a new point we read the data from file instead of reading it from database. I though that his idea was better implementation because if we have a lot of data (points) in the database it will take few milliseconds to get the response. But by saving it in a JSON file we can secure that get the data in a faster way.
 
---

## 2022-04-28 Thursday
 
Abdel and I met today. Abdel's get last point function sparked a lengthy debate regarding whether or not Abdels implementation was the most optimal way me and Abdel could implement. There was a second way I could implement the feature. Rather than pulling data from the database each time we want to add a new point, I came up with the idea of storing the most recent point in a JSON file first, and then adding it to the database after that. If we have a lot of data in the database, Abdel told me, it will take a few milliseconds for the response to come back, which is why he thinks the proposal is best implemented. However, by storing it in a JSON file, we can ensure that even with a large database, we can retrieve the data quickly.
 
---

## 2022-04-29 Friday
 
Our first meeting of the day was a discussion of the current sprint's accomplishments and plans for the upcoming one.
In this sprint, I was unable to complete a new assignment other than continuing to work on the classification features.

---

## 2022-05-03 Tuesday

A new database map feature will soon be added to the database after Abdel and Joshua and I agreed to start working on an additional feature.

I started to work on the classification functionality. i needed to to do many stuff such as writing the code as well as setting up every thing in the cloud service.

this day i started with setting up every thing in the cloud service.

---

## 2022-05-04 wednesday

This day me and Abdel started with writing the code that received an image and then sends the data to the cloud service to classify it and then upload the classification alongside with the image to firebase. 

---

## 2022-05-04 thuseday

I wrote unit test code to test the code i have implemented and then made a pull request

---

## 2022-05-06 Friday

We had a meeting where we discussed what we did in this sprint and what we would do in the next. I am open to new functionalities.

---

## 2022_05_10 Tuesday

I worked on **createMap()** in the data_access_layer wich means creating a map in firebase . 

---
## 2022_05_12 Thursday

I worked on **createMap()** in the testing layer to ensure the code is valid but i did not have the time to make a pull request.

---
## 2022-05-13 Friday

Even though the meeting was canceled, we all recorded our activities in our group discord server, which we use to stay in touch.

---

## 2022-05-17 Tuesday

me and Abdel worked on a bug where the niether the mower or the mobile team could comunicate with the server. After more than 3 hours I could found find one of the bugs in the code. so i made a pull request and added every thing github.

---
## 2022-05-19 Thursday

First, we upgraded the server with the new code version, and then we ran the mower and mobile teams through their paces. Some of the features did not perform as planned, so the development teams set to work correcting them.

---
## 2022-05-20 Friday

We continued our functional testing today. I and other members of the team have begun writing the necessary technical aspects and analyses and some required paperwork while others are testing.
In order to use these images in the presentation, we filmed and recorded the mower and the mobile screen.