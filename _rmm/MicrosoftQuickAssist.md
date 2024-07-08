---
Name: Microsoft Quick Assist
Description: Microsoft Quick Assist is a remote desktop tool. It communicates over port 443 (https) and connects to the Remote Assistance Service at https://remoteassistance.support.services.microsoft.com by using the Remote Desktop Protocol (RDP). The traffic is encrypted with TLS 1.2. 
Author: Microsoft
Website: https://learn.microsoft.com/en-us/windows/client-management/client-tools/quick-assist
Created: "2024-07-06"
Platforms:
  - Platform: Windows
    Full_Path:
      - Path: \%WINDIR\%\system32\quickassist.exe     
    Privileges: User
MitreIDs:
  - MitreID: T1219
Domains:
  - Domain: remoteassistance.support.services.microsoft.com
Ports:
  - Port: 443  
Detection:
  - Sigma:
  - IOC: 
Remediations:
  - Remediation: Blocking `remoteassistance.support.services.microsoft.com` prevents Quick Assist connections.
Resources:
  - Link: https://learn.microsoft.com/en-us/windows/client-management/client-tools/quick-assist#disable-quick-assist-within-your-organization
Tags:
  - RMM
Acknowledgement:
  - Person:
    Handle:
---