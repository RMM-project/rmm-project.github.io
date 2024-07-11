---
Name: Remote Utilities
Description: Remote Utilities is a tool that offers remote access to devices. This can be direct connections or access via the internet.
Author: Remote Utilities
Website: https://www.remoteutilities.com
Created: "2024-07-10"
Platforms:
  - Platform: Windows
    Full_Path:
      - Path: \%PROGRAMFILES(X86)\%\Remote Utilities - Host\
      - Path: \%PROGRAMFILES(X86)\%\Remote Utilities - Server\
      - Path: \%PROGRAMFILES(X86)\%\Remote Utilities - Viewer\
    Privileges: User
Ports:
  - Port: TCP 443 Inbound (Host) public server, in case port 5655 is blocked
  - Port: TCP 443 Outbound (Viewer) public server, in case port 5655 is blocked
  - Port: TCP 5650 Inbound (Host/Agent) direct connection,  default port can be changed
  - Port: TCP 5650 Outbound (Viewer) direct connection, default port can be changed  
  - Port: TCP 5655 Inbound (Host) public server
  - Port: TCP 5655 Outbound (Viewer) public server
  - Port: TCP 5670 Inbound (RU Server PC)
  - Port: TCP 5670 Outbound (Admin console PC)
MitreIDs:
  - MitreID: T1219
Domains:
  - Domain: id.remoteutilities.com
  - Domain: server.remoteutilities.com
  - Domain: \*.remoteutilities.com
Detection:
  - Sigma:
  - IOC: 
Remediations:
  - Remediation: Blocking `id.remoteutilities.com` blocks the connection to the internet relay server.
Resources:
  - Link: https://ics-cert.kaspersky.com/media/TV_RMS_PHISHING_EN.pdf
Tags:
  - RMM  
Acknowledgement:
  - Person:
    Handle:
---