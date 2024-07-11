---
Name: RemotePC
Description: RemotePC is a remote desktop and remote support software that enables you to remotely access and control apps, files, and data. 
Author: RemotePC
Website: https://www.remotepc.com/
Created: "2024-07-10"
Platforms:
  - Platform: Linux  
    Privileges: 
  - Platform: MacOS 	  
    Privileges: 	
  - Platform: Windows	  
    Privileges: User	  
MitreIDs:
  - MitreID: T1219
Domains:
  - Domain: remotepc.com
Ports:
  - Port:443
Detection:
  - Sigma:
  - IOC: 
Remediations:
  - Remediation: Blocking `*.remotepc.com` prevents RemotePC connections.
Resources:
  - Link: https://www.remotedesktop.com/helpdesk/faq-firewall
Tags:
  - RMM
Acknowledgement:
  - Person:
    Handle:
---