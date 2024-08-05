# Splunk-log-analysis

## Splunk-log-analysis: Comprehensive Search Queries

This repository provides a collection of search queries for analyzing system and security event logs in Splunk. By leveraging these queries, you can effectively gain valuable insights from your log data and identify potential security threats, track system performance, and troubleshoot issues efficiently.

### Objective

* Equip users with essential Splunk search queries to analyze system and security event logs.
* Enable users to monitor system health, identify security risks, and troubleshoot problems quickly.

### Skills Learned

* **Splunk Log Analysis:** Gain practical experience with Splunk search syntax and commands.
* **Event Log Interpretation:** Understand the structure and meaning of different event log types.
* **Security Monitoring Best Practices:** Learn best practices for monitoring security events in Splunk.

### Provided Searches

This repository offers a variety of pre-built search queries to target different system and security events. Each search includes a description and explanation:

1. **Search for Specific Event IDs:** Retrieve events based on specific event codes (e.g., successful and failed login attempts).
2. **Search for Logins by User:** Identify login activity for a particular user.
3. **Search for Failed Logins:** Focus on failed login attempts for potential security concerns.
4. **Search for Logins by IP Address:** Track login activity originating from specific IP addresses.
5. **Search for Account Lockouts:** Identify instances where user accounts have been locked.
6. **Search for System Startup/Shutdown Events:** Monitor system boot and shutdown activities.
7. **Search for Specific Error Codes:** Investigate events based on predefined error codes.

### Using the Provided Searches

These pre-built searches can be used as a starting point for your Splunk investigations. You can easily modify and combine them to create more specific searches tailored to your needs.

**Note:** While Splunk Enterprise was used for this exercise, these core search principles can be applied to various Splunk versions.

### Instructions for Setting Up Splunk Data Source 

**This section is included for reference**

This section provides a basic guide to adding data sources in Splunk Enterprise (http://127.0.0.1:8000).

1. Navigate to the **Settings** tab and click **"Add Data."**
2. Select the **"monitor"** icon.
3. Choose to monitor **"local events logs"** and select the desired logs (e.g., security, system).
4. Review settings and click **"Submit."**
5. Click **"Start searching your data"** to begin analyzing collected logs.


### Additional Notes

* Feel free to contribute additional search queries to this repository.
* Explore more advanced Splunk features for further log analysis capabilities.
* Always refer to Splunk documentation for detailed information on search syntax and functionalities.


