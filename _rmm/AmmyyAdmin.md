---
Name: Ammyy Admin
Description: Ammyy Admin is used for system administration, webinars and instant remote desktop connection over the Internet.
Author: Ammyy
Website: https://wwww.ammyyy.com
Created: "2024-07-06"
Platforms:
  - Platform: Windows
    Privileges: User
MitreIDs:
  - MitreID: T1219
Domains:
  - Domain: rl.ammyy.com
Detection:
  - Sigma:
  - IOC: 
Remediations:
  - Remediation: Blocking `rl.ammyy.com` prevents all Ammyy Admin functionality for both outgoing connections from clients on your network and incoming connections to hosts on your network. Though not necessary if the API is blocked, you can also block `ammyy.com` to prevent the client from being loaded.   
Resources:
  - Link: https://www.exploit-db.com/exploits/34647
Tags:
  - RMM
Acknowledgement:
  - Person:
    Handle:
---