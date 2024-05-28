# Splunk-log-analysis
Comprehensive Search Queries for System and Security Event Logs

Objective:
The objective of this repository is to provide users with a comprehensive collection of search queries for analyzing system and security event logs in Splunk. By leveraging these queries, users can effectively monitor and extract valuable insights from their log data, enabling them to identify potential security threats, track system performance, and troubleshoot issues efficiently.

Skills Learned:
- Splunk log analysis and monitoring.
- Understanding of event log data structure and interpretation.
- Familiarity with event log monitoring best practices and security protocols.

Searches to include:

1. Search for Specific Event IDs:
This search retrieves all security events with Event IDs 4624 (successful logins) and 4625 (failed logins).
   
   index=main sourcetype="WinEventLog:Security" EventCode=4624 OR EventCode=4625
   

2. Search for Logins by a Specific User:
Replace "username" with the username you want to search for. This search retrieves successful login events for the specified user.
   
   index=main sourcetype="WinEventLog:Security" EventCode=4624 Account_Name="username"
   

3. Search for Failed Logins:
This search retrieves all security events indicating failed login attempts.
   
   index=main sourcetype="WinEventLog:Security" EventCode=4625
   

4. Search for Logins from Specific IP Addresses:
Replace "192.168.1.15" with the IP address you want to search for. This search retrieves successful login events from the specified IP address.
   
   index=main sourcetype="WinEventLog:Security" EventCode=4624 Source_Network_Address="192.168.1.15"
  

5. Search for Account Lockouts:
This search retrieves security events indicating account lockouts.

   index=main sourcetype="WinEventLog:Security" EventCode=4740

6. Search for System Startup and Shutdown Events:
This search retrieves events indicating system startup (EventCode=6005) and shutdown (EventCode=6006).
   index=main sourcetype="WinEventLog:System" EventCode=6005 OR EventCode=6006

7. Search for Specific Error Codes:
This search retrieves events with the specified Event Code from the system event logs.
  
   index=main sourcetype="WinEventLog:System" EventCode=100


Instructions:
Splunk enterprise was used to complete this exercise. Login to your Splunk web interface (http://127.0.0.1:8000).

1. Go to the Settings tab and click "Add Data."

![image](https://github.com/Cipher-Rachael/Splunk-log-analysis/assets/101173177/3fa85fb1-33fb-4730-b308-286b5963fa2a)

2. Select the monitor icon.

![image](https://github.com/Cipher-Rachael/Splunk-log-analysis/assets/101173177/60a1ef4a-1b1e-4dbd-8743-890845f9a039)

3. Choose to monitor local events logs and add security and system logs, then click "Next."

![image](https://github.com/Cipher-Rachael/Splunk-log-analysis/assets/101173177/d41c566e-9773-45e5-8f69-132480baa523)

4. Review the settings and click "Submit."
   
![image](https://github.com/Cipher-Rachael/Splunk-log-analysis/assets/101173177/1e694d6a-0567-48f7-b3a7-8c853637c640)

5. Click on "Start searching your data" to begin analyzing the collected logs.

![image](https://github.com/Cipher-Rachael/Splunk-log-analysis/assets/101173177/34f7a407-2108-4b05-8cd3-ae94a5997591)

6. The results will be generated as per below. On the search bar you can generate more searches like the ones mentioned and more.

![image](https://github.com/Cipher-Rachael/Splunk-log-analysis/assets/101173177/b8797c89-bbb4-4963-8013-ff17dbd03ba3)

These are some of the search results:

Specific Id's:

![image](https://github.com/Cipher-Rachael/Splunk-log-analysis/assets/101173177/b1e5c152-4721-4c27-a1d1-555d7f8a486c)

Failed login attempts:

![image](https://github.com/Cipher-Rachael/Splunk-log-analysis/assets/101173177/2cbfa8ad-2156-4b6e-aa9b-aaf5c5cd3044)

System startup and shutdown

![image](https://github.com/Cipher-Rachael/Splunk-log-analysis/assets/101173177/3c8f4fba-e3e3-41b4-9e30-172df3103cbb)



This repository serves as a valuable resource for individuals and organizations seeking to enhance their log analysis capabilities in Splunk. By providing a curated collection of search queries for system and security event logs, users can streamline their monitoring processes, detect anomalies, and mitigate security risks effectively. By leveraging these tools and skills, users can maintain the integrity, security, and performance of their systems while gaining actionable insights from their log data. The data can however be filtered for accuracy and desired outcome.
