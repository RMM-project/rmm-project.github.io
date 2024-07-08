---
Name: Anydesk
Description: Anydesk is a remote desktop tool.
Author: Anydesk
Website: https://anydesk.com
Created: "2024-07-08"
Platforms:
  - Platform: Windows
    Full_Path:
      - Path: \%PROGRAMDATA\%\AnyDesk
      - Path: \%APPDATA\%\AnyDesk
    Privileges: User
MitreIDs:
  - MitreID: T1219
Domains:
  - Domain: anydesk.com
Detection:
  - Sigma:
  - IOC: 
Remediations:
  - Remediation: Blocking `anydesk.com` prevents all Anydesk functionality for both outgoing connections from clients on your network and incoming connections to hosts on your network.   
Resources:
  - Link: https://www.mediarealm.com.au/articles/block-anydesk-network-guide/
Tags:
  - RMM
Acknowledgement:
  - Person:
    Handle:
---