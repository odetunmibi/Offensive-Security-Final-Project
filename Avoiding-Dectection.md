# Avoiding Detection 
## Stealth Exploitation WordPress/WPScan
### Monitoring Overview
- The Excessive HTTP Errors alert detected this exploit. 
- This alert measures the count of the top 5 https response codes.
- The alert will fire when it reaches a threshold of 400 in the last 5 minutes.

### Mitigating Detection
- To avoid triggering the alert, different options can be utilized to break up the scan, such as --stealthy which has a passive detection mode and uses a random user agent. 
- An alternative exploit that may perform better would be nmap with the -sS option because it can be quickly performed and is relatively stealthy as it never completes TCP connections.
## Stealth Exploitation of Brute Force
### Monitoring Overview
- The Excessive HTTP Errors alert detected this exploit. 
- This alert measures the count of the top 5 https response codes.
- The alert will fire when it reaches a threshold of 400 in the last 5 minutes.

### Mitigating Detection
- To avoid triggering the alert, an outer perimeter remote stealth pass brute force can be executed in which the password is brute forced offline and no record of an invalid login attempt is created.
- An alternative exploit that may perform better would be to utilize nmap and john-the-ripper.
## Stealth Exploitation of Privilege Escalation
### Monitoring Overview
- An alert set up to monitor functions of AuditBeat can detect specific login information, such as per user or a number of attempts.
- The alert could be set up to trigger on one login to the root account, at any point in time, from any IP.
### Mitigating Detection
- Using tools like hydra will helpful in avoiding login attemps while using a bruforce tool without detction.
- Using AWS as a server tricks company users to thinking its one of them. (Cloud as a Service.)
