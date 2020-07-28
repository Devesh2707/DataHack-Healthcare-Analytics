# JanataHack:Healthcare Analytics
### Problem Statement
***
MedCamp organizes health camps in several cities with low work life balance. They reach out to working people and ask them to register for these health camps. For those who attend, MedCamp provides them facility to undergo health checks or increase awareness by visiting various stalls (depending on the format of camp). 

MedCamp has conducted 65 such events over a period of 4 years and they see a high drop off between “Registration” and Number of people taking tests at the Camps. In last 4 years, they have stored data of ~110,000 registrations they have done.

One of the huge costs in arranging these camps is the amount of inventory you need to carry. If you carry more than required inventory, you incur unnecessarily high costs. On the other hand, if you carry less than required inventory for conducting these medical checks, people end up having bad experience.

#### The Process
1. MedCamp employees / volunteers reach out to people and drive registrations.
2. During the camp, People who “ShowUp” either undergo the medical tests or visit stalls depending on the format of health camp.

#### Favorable outcome
* For the first 2 formats, a favourable outcome is defined as getting a health_score, while in the third format it is defined as visiting at least a stall.
* You need to predict the chances (probability) of having a favourable outcome.

### Data Description
***
#### Train.zip contains the following 6 csvs alongside the data dictionary that contains definitions for each variable:
Health_Camp_Detail.csv – File containing Health_Camp_Id, Camp_Start_Date, Camp_End_Date and Category details of each camp.

Train.csv – File containing registration details for all the test camps. This includes Patient_ID, Health_Camp_ID, Registration_Date and a few anonymized variables as on registration date.

Patient_Profile.csv – This file contains Patient profile details like Patient_ID, Online_Follower, Social media details, Income, Education, Age, First_Interaction_Date, City_Type and Employer_Category

First_Health_Camp_Attended.csv – This file contains details about people who attended health camp of first format. This includes Donation (amount) & Health_Score of the person.

Second_Health_Camp_Attended.csv - This file contains details about people who attended health camp of second format. This includes Health_Score of the person.

Third_Health_Camp_Attended.csv - This file contains details about people who attended health camp of third format. This includes Number_of_stall_visited & Last_Stall_Visited_Number.

#### Test Set:
Test.csv – File containing registration details for all the test camps. This includes Patient_ID, Health_Camp_ID, Registration_Date and a few anonymized variables as on registration date.

#### Train / Test split:
* Camps started on or before 31st March 2006 are considered in Train
* Test data is for all camps conducted on or after 1st April 2006.

### Evaluation Metric:
The evaluation metric for this hackathon is ROC-AUC Score.

### Result:
###### No. of registered: 14458
###### Public Leaderboard rank: 71
###### Private Leaderboard rank: 81
[Leaderboard](https://datahack.analyticsvidhya.com/contest/janatahack-healthcare-analytics/#LeaderBoard)
