<a href="https://github.com/sts07142/senior_project/GuardianWatch">WIKI</a>
# 2023 Gachon univ. SW senior_project '**GuardianWatch**'
***
# GuardianWatch
* ### A monitoring system uses AI and Multi-Object Tracking to overcome the limitations of safety management at childcare centers
* [GuardianWatch.pdf](https://github.com/sts07142/senior_project/files/11783818/1.C-1.pdf)<br>
* [Youtube](https://youtu.be/cxkx-hbuiXk)

> Members 
>> 201935085 유인재 <br>  202135588 최지우 <br> 201033095 김경민 <br> 201935011 김관일

***
# Index
### [1. Background & Motivation](https://github.com/sts07142/senior_project/GuardianWatch#1-background--motivation-1)
> [a. Background](https://github.com/sts07142/senior_project/GuardianWatch#a-background)<br>
> [b. Motivation](https://github.com/sts07142/senior_project/GuardianWatch#b-motivation)
### [2. Overview](https://github.com/sts07142/senior_project/GuardianWatch#2-overview-1)
> [Mobile APP UI](https://github.com/sts07142/senior_project/GuardianWatch#2Guardianwatchs-mobile-app-ui)
>> [1. Main](https://github.com/sts07142/senior_project/GuardianWatch#1-main)<br>
>> [2. Child List](https://github.com/sts07142/senior_project/GuardianWatch#2child-list)<br>
>> [3. Register child](https://github.com/sts07142/senior_project/GuardianWatch#3register-child)<br>
>> [4. Notification](https://github.com/sts07142/senior_project/GuardianWatch#4-notification)<br>
>> [5. Heat Map](https://github.com/sts07142/senior_project/GuardianWatch#5heat-map)<br>
>> [6. Activity Analysis](https://github.com/sts07142/senior_project/GuardianWatch#6activity-analysis)
### [3. System](https://github.com/sts07142/senior_project/GuardianWatch#3-system-1)
> [Development Components](https://github.com/sts07142/senior_project/GuardianWatch#development-components)<br>
> [Development Contents](https://github.com/sts07142/senior_project/GuardianWatch#development-contents)
### [4. Plan](https://github.com/sts07142/senior_project/GuardianWatch#4-plan-1)
### [5. Expectation](https://github.com/sts07142/senior_project/GuardianWatch#5-expectation-1)
***

# [1. Background & Motivation](https://github.com/sts07142/senior_project/GuardianWatch#Index)
## a. Background
* ### It is the recent increase in _**child abuse**_
* ### _**Reliability**_ problems in daycare centers
* ### Lack of _**safety management**_ measures
* ### Parents' _**curiosity**_ about their children.
## b. Motivation
* ### Despite the mandatory CCTV requirements for childcare centers, child abuse cases has continued to increase every year
* ### Despite the fact that various measures have been taken to prevent loopholes related to CCTV, <br> issues related to child abuse have continued to arise.
* ### In order to avoid legal responsibility for abuse, problems such as <br>_damage to CCTV storage devices_ or _refusal to submit_ them are occurring.
> ### Need for a new monitoring system that improved the shortcomings of the existing system <br> CCTV-related problems and managing data using public servers that others could not touch.

# [2. Overview](https://github.com/sts07142/senior_project/GuardianWatch#Index)
## - Intelligent Childcare Center Safety Monitoring System
## 1.Detect / Trace child's location and behavior and inform your guardian of your child's situation in real-time
* ## Children may not be able to properly convey their situation to their parents or guardians due to lack of communication skills
> First, preventing harmful situations that can occur because children cannot explain them in words<br>
Second, allowing teachers and parents to quickly understand and respond to their children's situations<br><br>
And through this, information on individual characteristics, activity volume, situation, and status analyzed is provided to parents and managers.<br>
This will allow students to receive education in a safer environment, and parents and teachers will be able to manage their children in a more efficient system.
## [2.GuardianWatch's Mobile APP UI](https://github.com/sts07142/senior_project/GuardianWatch#Index)
### 1. Main
![image](https://github.com/sts07142/senior_project/assets/87844358/c7441cfe-b280-4207-88f4-66a69116e9b9)
### 2.Child List
![image](https://github.com/sts07142/senior_project/assets/87844358/8dfba726-f533-4d1a-b492-e4692b9b8df4)
### 3.Register child
![image](https://github.com/sts07142/senior_project/assets/87844358/98106cf8-e7f2-4d31-820b-934bfeda4010)
### 4. Notification
![image](https://github.com/sts07142/senior_project/assets/87844358/47c33803-bc26-4b67-be5f-805660190720)
### 5.Heat Map
![image](https://github.com/sts07142/senior_project/assets/87844358/cf2486a0-ba1b-4de6-9607-c5097e11d9e8)
### 6.Activity Analysis
![image](https://github.com/sts07142/senior_project/assets/87844358/9a0cde53-6fa5-4360-ab5e-23a37073c1ad)

# [3. System](https://github.com/sts07142/senior_project/GuardianWatch#Index)
* ## Overall System Implementation Projections
![image](https://github.com/sts07142/senior_project/assets/87844358/d58eb6d3-e74f-493b-899f-7346f6d1d0da)
### 1.In this system, children's video information is transmitted to the server in real time through CCTV at the childcare center.
### 2.These image information is analyzed by MOT technology on the server, and individuals are identified using object matching technology using Bluetooth tags, and information of each object is stored in the DB.
### 3.The analysis is sent as a notification to the client app via post-processing.

* ## [Development Components](https://github.com/sts07142/senior_project/GuardianWatch#Index)
### 1. Servers
> * Video Analysis Server<br>
> * DB Mapping Server<br>
> * Post-processing Server

### 2. Databases
> * Real-time Video Database<br>
> * Analysis Info Database

### 3. Algorithms
> * Video Analysis AL
> * Object Matching AL
> * HeatMap AL

### 4. Client APP
> * Receive Notification
> * Confirm Situation

* ## [Development Contents](https://github.com/sts07142/senior_project/GuardianWatch#Index)
### 1. Software
> * YOLO
>> * Multiple-Object Tracking
>> * Byte Track

### 2. Hardware
> * CCTV
> * Blutetooth Tag

### 3. System Goals
> * Danger detection system
> * Tracking all activities of kids in childcare center

### 4. Anticipated Users
> * Parents
> * Teachers in childcare center


# [4. Plan](https://github.com/sts07142/senior_project/GuardianWatch#Index)
* ## Montly
![image](https://github.com/sts07142/senior_project/assets/87844358/f7153715-6c95-4517-a5b8-799b40a60b16)
* ## Weekly
![image](https://github.com/sts07142/senior_project/assets/87844358/be79da46-a034-4736-8e07-aaeb3639f205)

# [5. Expectation](https://github.com/sts07142/senior_project/GuardianWatch#Index)
### 1. Political conflict
> It seems that it can be solved by creating a consent form to use the Guardian Watch. We hope that only those who have approved this agreement will be able to make the system available to them, thereby compromising legal issues. In addition, since actual image information is masked and delivered through location tracking, it is expected that it will be able to cope with problems related to personal information.

### 2. Understanding & Communication
> The Guardian Watch informs parents who are unable to observe their children because of their work. Through digitized/visualized records, parents will be able to know the personality and behavior of their children that they have not yet confirmed, and we expect that this will be a necessary guideline for parents to understand and communicate with their children.

### 3. Effective education
> The information obtained from the Guardian Watch can be used to understand the behavioral patterns and personalities of the students, and through this, effective education methods tailored to individual characteristics can be planned. This information is expected to help teachers understand the growth and development of the students.

### 4. Preventing accidents
> Guardian Watch can play a big role in preventing accidents for students. Even when guardians or teachers do not see it, the Guardian Watch informs the crisis in real time through video analysis to help prevent accidents or respond quickly.

### 5. Educational research
> Children's behavioral data collected by the Guardian Watch can be valuable data that contributes to improving the education system. I think this can be of great help in promoting new theories and insights related to child development and education.

### 6. Customized management
> Guardian Watch can play a big role in creating a more efficient proto-care environment. It is possible to analyze each student's activities to create a personalized learning environment, or to optimize the educational curriculum that oversees them. This can compensate for the chronic shortcomings of daycare centers that operate organizations as one.
