---
Name: GoToMyPC
Description: GoToMyPC is a company that offers remote access software and services.<br> The LogMeIn software uses a proprietary remote desktop protocol that is transmitted over SSL.<br> Users access the machines associated with LogMeIn using a proprietary application or via the web portal.
Author: GoToMyPC
Website: https://www.gotomypc.com
Created: "2024-07-10"
Platforms:
  - Platform: Windows
    Privileges: User
MitreIDs:
  - MitreID: T1219
Domains:
  - Domain: \*.gotomypc.com  
  - Domain: poll.gotomypc.com
IPs:
  - IP: "66.151.158.177"
Detection:
  - Sigma:
  - IOC: 
Remediations:
  - Remediation: ???
Resources:
  - Link: https://community.cisco.com/t5/network-security/asa-5520-and-blocking-logmein-and-gotomypc/td-p/1529887
  - RMM
Acknowledgement:
  - Person:
    Handle:
---