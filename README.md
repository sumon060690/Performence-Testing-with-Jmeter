# Project Summary:
## I have completed following task:
Create a JMeter collection (booking.jmx)
● Add the following properties to the Header Controller:
○ Accept: */*
# Login:
○ URL: https://restful-booker.herokuapp.com/auth
○ Body:
{
"username": "admin",
"password": "password123"
}

# Create Booking:
○ URL: https://restful-booker.herokuapp.com/booking
○ Body:
{
"firstname": "John",
"lastname": "Doe",
"totalprice": 100,
"depositpaid": true,
"bookingdates": {
"checkin": "2024-09-01",
"checkout": "2024-09-02"
}
}

# Search Booking:
○ URL: https://restful-booker.herokuapp.com/booking/<booking_id&gt;
Now, perform performance testing for the following scenario:

## Scenario:
120,000 users over a 12-hour period log in, create a booking, and search for the
booking.
# Todo 1:
Find the throughput and perform a load test (you can limit the load test to a maximum of
20 minutes to save time) to ensure the server can handle the load. Create a load test
report.
# Todo 2:
Identify the bottleneck throughput by conducting a stress test.
Create a stress test report.
# Todo 3:
Generate an HTML report for both the load test and the stress test.
2. From the dmoney API collection, create another JMeter collection (dmoney.jmx) for the
following scenario:

## Scenario:
○ 5 agents perform deposits for 10 customers.
○ 5 customers send money to another 10 customers.
○ 5 customers make payments to 2 merchants.
○ Create a separate thread for withdrawals, where you will generate a
withdraw.csv dataset by applying Boundary Value Analysis (BVA) for the
withdrawal amount. Set the ramp-up time to 120 seconds in the thread
configuration.

# HINT:
Log in as an admin once and generate a token to use. Create 4 threads for each type of
transaction and set up agent, customer, and merchant accounts in 4 different CSV files
(e.g., deposit.csv, sendMoney.csv, payment.csv and withdraw.csv). The
amount must be dynamic using the Random Variable Controller, but for the withdrawal
scenario, get a specific amount from the CSV that was calculated using the BVA
strategy. Each thread should have a ramp-up time of 120 seconds.Submission Process:
1. I have Upload my folder to GitHub. The folder is include the following files:
○ booking.jmx
○ dmoney.jmx
○ deposit.csv
○ withdraw.csv
○ sendMoney.csv
○ payment.csv
2. Add dmoney.jtl and the HTML report folder to .gitignore.
3. Writing necessary information in the README.md file, including what you have done,
prerequisites, and instructions on how to run the tests.
4. Generate the report and taking screenshots of the request summary and statistics.
5. Add the screenshots of the request summary, statistics, and the two reports (load test
and stress test) in the README.md for Question 1.
For Question 2, add only the screenshots of the request summary and statistics from
the generated HTML report.

Please follow the attached link for the assignment.

## Load Test:
![Screenshot 2024-11-04 221250](https://github.com/user-attachments/assets/ce8b9d4f-789d-46e1-b01d-20627085dca2)
![Screenshot 2024-11-04 221235](https://github.com/user-attachments/assets/ad2a3426-ecd3-4c60-8095-dd6247552503)
![Screenshot 2024-11-04 221250](https://github.com/user-attachments/assets/36814cc5-57a9-45f0-badb-ec2cef26a063)

## Stress Test:
![Screenshot 2024-11-04 221446](https://github.com/user-attachments/assets/f9daa210-507b-47c6-b00e-e94b43d8bbd6)
![Screenshot 2024-11-04 221507](https://github.com/user-attachments/assets/1151a7b0-a910-4c7b-9b0f-a583572c17f2)
![Screenshot 2024-11-04 221518](https://github.com/user-attachments/assets/c6ae4d85-fb5b-4799-b7a5-e0d0d6f0e78c)



## DMoney API collection request
![image](https://github.com/user-attachments/assets/ec91322b-0943-4e70-9c41-35705080f456)





