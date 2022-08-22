# retention_prediction_sql

## Description of database and task

### Database
On the picture you can see a database which was used for this task. It consists of 4 different tables.

![image](https://user-images.githubusercontent.com/77459095/185864184-05cd9269-cd3d-4dd4-85dc-510d49480fdd.png)

1.regular_users - users who came to our social platform to get valuable information from influencers, watch their videos or streams, talk to them. Most fields are intuitively clear, but others might not be, so:
- mirror_group - region of user
- email_vendor - which email user uses (gmail, yahoo...)
2.trusted_users - influencers, who share their content on platform.
3.logins - when, from which platform, how many times user came.
4.messages - how many, when and to who regular user was writing messages.

### Tasks
1. Build a user retention curve (Rolling Retention). What percentage returned on any day from N to 30, where N = {0, 1, 2 ... 14}.

2. Let's take users registered in [2019-01-15; 2019-01-31]. Build a prediction of how many messages they generate in total on the 15th day of life.

3. Build a matrix of audiences (by X RU_platform, by Y - RU_age), age values - 10% percentiles.
Fill in the received matrix:
1) Number of RUs
2) Percentage of RU from the total
3) retention of the 1st day
