# SIEM-Unusual-Login-Investigation
Beginner SOC investigation: analysing a suspicious login alert using SIEM methodology.
How I Investigated and tackled the unusual login alert
1. Reviewed the SIEM alert
I started by checking the alert details:
Login at 02:14 AM
Foreign IP address
Multiple failed attempts
No successful login afterwards
This helped me understand the severity.

2. Analysed the Login Behaviour
I checked: The time of login (outside normal hours)
The IP location (foreign country)
The number of attempts (too many)
The failure reason (bad password)
These are strong indicators of brute‑force activity.

3. Checked SIEM Logs
I looked at: Authentication logs
User activity logs
IP reputation
I found: 12 failed attempts IP flagged as suspicious
No legitimate user activity around that time
This confirmed the login was not normal user behaviour.

4. Checked Threat Intelligence
I searched the IP address: Known for malicious activity
Associated with brute‑force attempts
Medium‑high risk
This validated the threat.

5. Took Recommended SOC Actions
I recommended: Locking the account
Resetting the password
Blocking the IP Enforcing MFA Monitoring for further attempts
Notifying the security team These steps protect the user and prevent account compromise.
