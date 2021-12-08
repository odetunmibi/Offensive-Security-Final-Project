# Network topology 

The Hyper V machine used consist many VM’s on its server:

2 attack machines, 

Vulnerable Web Server

ELK Machine
an Attacker Machine.
## Answer
![Image1](/images/Image1.png)

# Critical Vulnerabilities

The following vulnerabilities were identified on each target:

Target 1:

- Directory Listing

- Brute Force

- Privilege Escalation

| Vulnerability        | Description           | Impact  |
| ------------- |:-------------:| -----:|
| Directory Listing/Sensitive Data Exposure| The ability to view directory contents on a website, rather than the html | Search and information gathering past what the developer intended |
| Brute Force/WPScan     | As long as a username is known, a password (especially weaker) can be found through trial and error      |   Access to ‘michael’ useraccount by enumerating with WPScan and guessing the password
 |Privilege Escalation | The ability to elevate from a user account to an admin or root account with higher privilege    |    An admin or root account has carte blanche, no restrictions |
