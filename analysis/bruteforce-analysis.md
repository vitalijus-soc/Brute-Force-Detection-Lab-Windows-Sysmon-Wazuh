# Brute-Force Activity Analysis

## What happened
Multiple failed login attempts (Event ID 4625) were generated within a short time window using a test account.

## Why it's suspicious
Single failed logins are normal, but repeated rapid failures indicate possible brute-force or credential guessing activity.

## How detected
Wazuh detected multiple Event ID 4625 logs and correlated them into a high-severity alert:

Rule ID: 60204  
Description: Multiple Windows logon failures  
Level: 10
