## Project Description

The commercial department of a telecom operator mega line wants to know which plans among the two prepaid plan they offer brings more revenue in order to adjust advertising budget

**Task: Analyse client’s behaviour and determine which plan brings more revenue** 


**Plans Description:**
Megaline rounds seconds up to minutes, and megabytes to gigabytes. For calls, each individual call is rounded up: even if the call lasted just one second, it will be counted as one minute. For web traffic, individual web sessions are not rounded up. Instead, the total for the month is rounded up. If someone uses 1025 megabytes this month, they will be charged for 2 gigabytes.

1. Surf
- Monthly charge: 20 dollars
- 500 monthly minutes, 50 texts, and 15 GB of data
- After exceeding the package limits:
    - 1 minute: 3 cents
    - 1 text message: 3 cents
    - 1 GB of data: 10 dollars

2. Ultimate
- Monthly charge: 70 dollars
- 3000 monthly minutes, 1000 text messages, and 30 GB of data
- After exceeding the package limits:
    - 1 minute: 1 cent
    - 1 text message: 1 cent
    - 1 GB of data: 7 dollars


### Data Description


The users table (data on users):
1. user_id — unique user identifier
2. first_name — user's name
3. last_name — user's last name
4. age — user's age (years)
5. reg_date — subscription date (dd, mm, yy)
6. churn_date — the date the user stopped using the service (if the value is missing, the calling plan was being used when this data was retrieved)
7. city — user's city of residence
8. plan — calling plan name

The calls table (data on calls):
1. id — unique call identifier
2. call_date — call date
3. duration — call duration (in minutes)
4. user_id — the identifier of the user making the call
5. The messages table (data on texts):
6. id — unique text message identifier
7. message_date — text message date
8. user_id — the identifier of the user sending the text

The internet table (data on web sessions):
1. id — unique session identifier
2. mb_used — the volume of data spent during the session (in megabytes)
3. session_date — web session date
4. user_id — user identifier

The plans table (data on the plans):
1. plan_name — calling plan name
2. usd_monthly_fee — monthly charge in US dollars
3. minutes_included — monthly minute allowance
4. messages_included — monthly text allowance
5. mb_per_month_included — data volume allowance (in megabytes)
6. usd_per_minute — price per minute after exceeding the package limits (e.g., if the package includes 100 minutes, the 101st minute will be charged)
7. usd_per_message — price per text after exceeding the package limits
8. usd_per_gb — price per extra gigabyte of data after exceeding the package limits (1 GB = 1024 megabytes)
