# Survival-analysis-in-football-player-injury
This is final project in my class (CPE352 - Data Science)

## objective
i want to know when football player face with the most severe injury in his career,How long when they will injury again(same injury and different injury both include in this project)

## Detail 
i use dataset from https://www.kaggle.com/eliesemmel/kernelde4fae5abe to run model

this project have 3 steps 

1.prepare dataset for model by find the most severe injury and next injury they face.

2.fit KaplanMeier model to check trend to comeback with injury

3.fit Cox proportional hazard model to create machine learning that can predict how long untill player comeback again.

## Result and conclusion

-KaplanMeier model show most player will have injury again in one year

-Cox PH model have concordance score = 0.72

## Discussion
in this project that have weak point are

1.in this project i include recovery time in time to return that mean if player have severe and use much time to recovery(ex. ACL injury 1 year) time untill they return will incorrect(because it have recovery time in that).

2.in Cox PH model i choose use type of injury in factor to teach machine,that can improve performance of this ML.

3.for complete conclusion,I should seperate in 2 case are player who injury in same cause and injury in other cause.
