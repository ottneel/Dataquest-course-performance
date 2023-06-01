# Dataquest-course-performance
### INTRODUCTION
In this Project, I assume the position of a business analyst at Dataquest tasked with analyzing the performance of DQ courses and to make recommendations based on Data on 5 course that should be improved.

This project has three data tables, stored as CSVs.

Mission Progress Data

missionprogress_id — a unique ID for the user and the lesson
started_at — the date and time the learner started the lesson
lession_id — a unique ID for a lesson
is_complete — a Boolean (True/False) for whether the learner completed the lesson
completed_at — the date and time when the learner completed the lesson

NPS Survey Data

response_id — a unique ID for the NPS survey response
date — the date when the learner submitted their survey response
score — the learner's response to the question "On a scale of 1-10, how likely are you to recommend Dataquest to someone interested in learning data skills?"


Lesson and Course Structure Data

lesson_id — a unique ID for a lesson
course_id — a unique ID for a course.


**UNDERSTANDING THE PROBLEM**
The basic questions I'd be answering are:
1. How are dataquest courses performing?
2. Which 5 courses will I recommend to the Dataquest board

**DATA PREPARATION**

Prepared the dataset using Powerquery editor in PowerBI. Extracted the columns with null values in each column, Changed the datatype for the lesson_ids, resolved data inconsistencies and confirmed that every other column was in perfect condition.


**DATA MODELLING**
Created a relationship between lesson IDs in the three tables.

**IMPORTANT MEASURES CREATED**
The first analysis i'll work on uses the lesson completion data. Lesson completion rate is a useful metric for understanding course quality. Lessons with high completion rates show that learners understand the curriculum and are engaged enough to complete the lesson. Low completion rates suggest there may be an issue that needs to be addressed.


Net promoter score (NPS) is a common metric used across industries to measure customer satisfaction. You can read more about it [here](https://www.netpromoter.com/know/). The resulting metric gives you a number between -100 and 100. It's calculated from the results of a survey question that asks "On a scale of 1-10, how likely are you to recommend this product to others?"

To calculate NPS, you split the scores into three groups:

Promoters (response of 9 or 10) — These learners are enthusiastic about their experience and likely to refer it to others.

Passives (response of 7 or 8) — These learners are satisfied about their experience, but they're not quite loyal customers yet.

Detractors (response of 1-6) — These learners are unsatisfied and less likely to continue learning with Dataquest.

To get the final NPS score, you take the number of promoters, subtract the number of detractors, divide the difference by the total number of responses, then multiple it by 100.



**KEY TAKEAWAYS**
•• Completion rate over time was 76.5%

![Screenshot_20230419-203551](https://user-images.githubusercontent.com/101079280/233181927-fbb20183-c1b2-4a68-9fb9-70fbac576dcd.png)

•• An average of 19,725 lessons were taken by learners

![Screenshot_20230419-203617](https://user-images.githubusercontent.com/101079280/233182346-9e567899-571a-4482-aafd-b353cf2320c8.png)

•• Approximately 69% of lessons taken by students was completely.

![Screenshot_20230419-203645](https://user-images.githubusercontent.com/101079280/233182791-d8700b12-951f-4be4-85fe-29e582629422.png)

•• Despite a dip in the completion rate in March 2021, there has been a steady rise in the completion rate

![Screenshot_20230419-204411_1681933489576](https://user-images.githubusercontent.com/101079280/233183352-29041393-9cb8-45d7-b4fc-7ca351667bce.jpg)

•• Over 5k respondents gave DQ courses a score 10. This accounts for over 50% of respondents.

![Screenshot_20230419-204610](https://user-images.githubusercontent.com/101079280/233184576-a001850e-6234-46a3-9e6c-a7e15b77003f.png)




•• NPS score stood at 62.8
![Screenshot_20230419-205302](https://user-images.githubusercontent.com/101079280/233184998-742ff4de-f061-41e2-ac08-d362442575be.png)

**CONCLUSION and RECOMMENDATION**
Which courses should be improved?

While it's safe to say that DQ is doing a brilliant Job with the courses content as students generally like the lessons and are enthused to finish them. However some courses needs to be looked into. Courses **9,58,20,100 87** as they are courses with the worst NPS score (-100) and lessons with low completion rate (lessons 499 and 311 in courses 87 and 58 respectively). I'd also reommend that maybe the length of these courses or the difficulty level could be ajusted as these could be what is frustrating learners.

![Screenshot_20230419-205853](https://user-images.githubusercontent.com/101079280/233186393-d53521a7-8df4-42b9-ab19-7e07350cc427.png)


