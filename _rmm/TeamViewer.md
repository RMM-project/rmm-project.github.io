---
Name: TeamViewer
Description: TeamViewer is a remote desktop and remote support software that enables you to remotely access and control apps, files, and data
Author: Splashtop
Website: https://www.teamviewer.com
Created: "2024-07-10"
Platforms:
  - Platform: Windows
    Full_Path:
      - Path: \%PROGRAMFILES(X86)\%$\TeamViewer\
      - Path: \%PROGRAMFILES\%$\TeamViewer\	  
    Privileges: User
    Registry:
      - Key: HKLM\SOFTWARE\TeamViewer
      - Key: HKLM\SOFTWARE\WOW6432Node\TeamViewer
      - Key: HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall\TeamViewer
      - Key: HKLM\SOFTWARE\WOW6432Node\Microsoft\Windows\CurrentVersion\Uninstall\TeamViewer
MitreIDs:
  - MitreID: T1219
Domains:
  - Domain: \*.dyngate.com
  - Domain: \*.teamviewer.com
Detection:
  - Sigma:
  - IOC: 
Remediations:
  - Remediation: Blocking `*.teamviewer.com` and `*.dyngate.com` prevents TeamViewer connections and access to the product page.
Resources:
  - Link: https://serverfault.com/questions/780626/how-to-block-teamviewer
  - RMM
Acknowledgement:
  - Person:
    Handle:
---