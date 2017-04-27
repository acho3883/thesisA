# thesisA

author: Amanda
date:   8/3/2017
    
This repository has been created to work on my project.

WEEK 1
1.	Submitted Thesis Topic Registration Form
2.	Set up GitHub Account: @acho3883
3.	Learnt how to use GitHub to store my document

WEEK 2
1. Met Intersective representative
2. Explored learning environment for NEXT

    Meeting 1   15/03/2017

    I was assigned to analyse data under one of the Intersective's programs, NEXT. Their interns did simple data analysis on data for   other learning programs. Notified Phil to send us previous findings. Data has been collected since recently and nothing much have been found. I am registered into NEXT and is to explore NEXT in this coming week. Primary task would be to find out what the data could mean. Data sanitisation is still on-going, predicted to be done by next meeting. Data size is less than 2000. Many different types of data are being captured including chat.

    Meatball is still under testing. Phil and Nikki might show me meatball next week. It is a more specialised version of Practera, catering to students from different universities with different requirements. Secondary task would be to find out if real life meeting updates are feasible.

    Next meeting is scheduled to be either on 22/03/17 or 23/03/17.
    
WEEK 3
1. Met Intersective representative
2. Explored learning environment for NEXT
3. Received database
4. Installed R Studio and PostGre

WEEK 4
1. Submitted project proposal
2. Screened throught the database
3. Made notes on what the tables are, and what information they hold

WEEK 5
1.	Listed possible weblinks on Practera by clicking in one by one, then classify them by similar addresses (refer dissect url)
2.	Looked into the table with user logs. It turns out that the refer weblinks on that table contains not only Practera links, but also     other email hosts. Many of them are from China. (refer dissect url)
3.	I also looked into another table with details on video links, visibility, and purpose of posting it. Phil told me there was a           benchmark time to track whether students have watched the video. There was only one column indicating view time, which I’m not sure     whether it’s the benchmark or average students’ view time. There are also created and modified time which I suspected are start         viewing time and end viewing time. However, some of the modified time are before created time, proving my prediction wrong.             (refer core_stories)
4.	Found some possible missing data and non-useful tables (refer potential missing data)
5.  Wrote to make appointment with Intersective but they haven't got back to me.

WEEK 6
1. Extracted rows referring only to practera website and studied the relationship of it with its URI. The extracted data only        include activities from year 2015 to 2016, supporting my idea of the inexistence of a unified learning platform some time before.        There are actions by 2 groups of people, admin and participants. What I can do next is to separate admin actions and participant        actions for further analysis.
2. Extracted a list of participants based on a few asseumptions:
    (a) All participants were grouped
    (b) All participants' actions were recorded in the action logs
    (c) Anyone who did not log on to Practera using admin accounts are considered as ordinary participants.

MID-SEMESTER BREAK
1.	Mapped all team members to their teams, programs, institutions, and experiences.
2.	Linked participants to participant profiles and team details. I attempted to do that using 2 methods. The first one using   current_team_id in the user_profile table, in which many of them are NULL. Second one using team_id in the team table. Both gave me different outputs. There's created time on the team table but there's no created time on profile table so I couldn't make comparison.
3.	Eliminated participants with multiple groups, assuming they are mentors.
4.	Found that core_stats contains data regarding survey when I first open Practera. Indicated stats_id are 1-6, but team_stats range 1-11; hence not sure what they mean exactly, and how they derive the percentage. The actual survey that I need to answer has only 3 questions and they are same every time I open.
5.	It was found out that the analytic teams were recorded as participants, I included those because that could be part of their project.
6.	I have also linked the participants to assessment results, achievements, and progresses. Achievements output is left with 30 entries, which I doubt they are correct. It could be some 'NULL' column here and there, and my code somehow eliminated those entries.

#############################################################################
QUESTIONS FOR INTERSECTIVE

1. Are students allowed to join the programs multiple times?If possible, do they use their existing accounts and just registerd to different groups?
2. Are mentors using admin accounts or regular participant accounts?
3. There are 3 tables with model_id but they don't seem to be relatable to each other: achieve_achievement_conditions, achieve_achievement, and achieve_progresses. There are some everlaps but most of them are eiher completely different, or different models sharing same model_id. Do you have any idea how to relate them?
#############################################################################

WEEK7
1. Explored different participant filtering options.
2. Database corrupted. Reimported to a new workspace.
3. Discussion with Intersective.
4. Retrieved new list of participants, but yet to figure out how to filter out mentors.
5. Start writing scripts for basic plots in R.
##########################################################################################################

WEEK 8
1. 
