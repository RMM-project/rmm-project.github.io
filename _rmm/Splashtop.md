---
Name: Splashtop
Description: Splashtop is a remote desktop and remote support software that enables you to remotely access and control apps, files, and data
Author: Splashtop
Website: https://www.splashtop.com
Created: "2024-07-09"
Platforms:
  - Platform: Windows
    Full_Path:
      - Path: \%PROGRAMFILES(X86)\%\Splashtop\Splashtop Software Updater\SSUService.exe    
    Privileges: User
MitreIDs:
  - MitreID: T1219
Domains:
  - Domain: api.splashtop.com (gobal)
  - Domain: api.splashtop.eu (EU)
  - Domain: relay.splashtop.com (both)
  - Domain: sn.splashtop.com (both), for auto-update
  - Domain: update.splashtop.comm (both), for auto-update
  - Domain: update-g3.splashtop.com (both), for auto-update
  
Detection:
  - Sigma:
  - IOC: 
Remediations:
  - Remediation: Blocking `*.splashtop.com` and `*.splashtop.eu` prevents Splashtop connections and access to the product page.
Resources:
  - Link: https://www.reddit.com/r/Ubiquiti/comments/rkqroi/udm_pro_firewall_blocking_remote_desktop/
  - Link: https://kb.naverisk.com/en/articles/6663123-splashtop-security-configuration
Tags:
  - RMM
Acknowledgement:
  - Person:
    Handle:
---