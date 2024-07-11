---
Name: Zoho Assist
Description: Zoho Assist is a remote desktop and remote support software that enables you to remotely access and control apps, files, and data. 
Author: Zoho
Website: https://www.zoho.com
Created: "2024-07-10"
Platforms:
  - Platform: Windows	  
    Privileges: User
MitreIDs:
  - MitreID: T1219
Domains:
  - Domain: \*.zoho.com
  - Domain: \*.zohoassist.com
Ports:
  - Port:443
Detection:
  - Sigma:
  - IOC: 
Remediations:
  - Remediation: Blocking `*.zoho.com` and `*.zohoassist.com` prevents Zoho Assist connections and access to the product page.
Resources:
  - Link: https://www.manageengine.com/mobile-device-management-msp/help/asset_management/mdm_remote_troubleshoot.html
Tags:
  - RMM
Acknowledgement:
  - Person:
    Handle:
---