---
Name: Chrome Remote Desktop
Description: Chrome Remote Desktop is a remote desktop tool, using the Chrome Browser.
Author: Google
Website: https://remotedesktop.google.com
Created: "2024-07-06"
Platforms:
  - Platform: MacOS
    Full_Path:
      - Path: ~/Library/Application Support/Google/Chrome Remote Desktop
    Privileges: 
  - Platform: Windows
    Full_Path:
      - Path: \%PROGRAMFILES\%\Google\Chrome Remote Desktop\[VERSION]\remoting_start_host.exe
      - Path: \%PROGRAMFILES(X86)\%\Google\Chrome Remote Desktop\[VERSION]\remoting_desktop.exe
      - Path: \%PROGRAMFILES(X86)\%\Google\Chrome Remote Desktop\[VERSION]\remoting_host.exe                 
      - Path: \%PROGRAMFILES(X86)\%\Google\Chrome Remote Desktop\[VERSION]\remoting_start_host.exe
    Privileges: User
MitreIDs:
  - MitreID: T1219
Domains:
  - Domain: remotedesktop-pa.googleapis.com
  - Domain: remotedesktop.google.com
Detection:
  - Sigma:
  - IOC: 
Remediations:
  - Remediation: Blocking `remotedesktop-pa.googleapis.com` prevents all Chrome Remote Desktop functionality for both outgoing connections from clients on your network and incoming connections to hosts on your network. Though not necessary if the API is blocked, you can also block `remotedesktop.google.com` to prevent the web client from being loaded.   
Resources:
  - Link: https://support.google.com/chrome/a/answer/2799701?hl=en
  - Link: https://sketchymoose.blogspot.com/2020/03/a-study-of-chrome-remote-desktop_25.html
Tags:
  - RMM
Acknowledgement:
  - Person:
    Handle:
---