# Avoiding Detection 
## Stealth Exploitation WordPress/WPScan
### Monitoring Overview
- The Excessive HTTP Errors alert detected this exploit. 
- This alert measures the count of the top 5 https response codes.
- The alert will fire when it reaches a threshold of 400 in the last 5 minutes.

### Mitigating Detection
- To avoid triggering the alert, different options can be utilized to break up the scan, such as --stealthy which has a passive detection mode and uses a random user agent. 
- An alternative exploit that may perform better would be nmap with the -sS option because it can be quickly - performed and is relatively stealthy as it never completes TCP connections.
