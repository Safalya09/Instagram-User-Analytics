# Instagram-User-Analytics
# Instagram User Engagement Analysis

## Project Overview
This project involves analyzing Instagram user interactions and engagement using SQL. The goal is to provide valuable insights that can help the product, marketing, and investor teams at Instagram make data-driven decisions. The analysis focuses on user behavior, content engagement, and platform activity to help enhance the user experience and support business strategies.

## Tools Used
- **SQL** (MySQL)
- **MySQL Workbench**
- **Instagram User Data (Simulated Database)**

## SQL Tasks & Insights

### 1. Marketing Analysis
- **Loyal User Reward:** Identified the five oldest users on Instagram based on the registration date.
- **Inactive User Engagement:** Analyzed user activity to find users who have never posted a single photo.
- **Contest Winner Declaration:** Identified the user with the most likes on a single post and declared them as the contest winner.
- **Hashtag Research:** Analyzed post data to suggest the top five most commonly used hashtags on Instagram.
- **Ad Campaign Launch:** Determined the best day of the week to launch ads based on user registration data.

### 2. Investor Metrics
- **User Engagement:** Calculated the average number of posts per user and provided insights on user activity.
- **Bots & Fake Accounts:** Identified users who have liked every single photo, flagging potential bots or fake accounts.

## Objectives & Goals
- Provide insights to the marketing team for promotional strategies.
- Help the product team improve user engagement by identifying inactive users and rewarding loyal ones.
- Support investor metrics by calculating user engagement and identifying suspicious accounts.

## How to Use
1. **Set up MySQL Workbench**: Install and configure MySQL Workbench to interact with the database.
2. **Database Setup**: Load the Instagram user data into your MySQL database.
3. **Run SQL Queries**: Use the SQL queries provided in the project to extract the insights outlined in the tasks.
4. **Review Insights**: Analyze the output of each SQL query and draw conclusions based on the results.

## Example SQL Queries

### Loyal User Reward
```sql
SELECT user_id, user_name, registration_date
FROM users
ORDER BY registration_date ASC
LIMIT 5;
