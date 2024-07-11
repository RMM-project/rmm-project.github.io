---
Name: LogMeIn
Description: LogMeIn is a company that offers remote access software and services.<br> The LogMeIn software uses a proprietary remote desktop protocol that is transmitted over SSL.<br> Users access the machines associated with LogMeIn using a proprietary application or via the web portal.
Author: LogMeIn
Website: https://www.logmein.com
Created: "2024-07-10"
Platforms:
  - Platform: Windows
    Privileges: User
MitreIDs:
  - MitreID: T1219
Domains:
  - Domain: \*.123rescue.com  
  - Domain: \*.hamachi.cc
  - Domain: \*.internapcdn.net
  - Domain: \*.logme.in
  - Domain: \*.logmein.com
  - Domain: \*.logmeinrescue.com
  - Domain: \*.logmeinrescue-enterprise.com
Detection:
  - Sigma:
  - IOC: 
Remediations:
  - Remediation: Blocking `*.123rescue.com`, `*.hamachi.cc`, `*.logme.in`, `*.internapcdn.net`, `*.logmein.com`, `*.logmeinrescue.com`, `*.logmeinrescue-enterprise.com` prevents LogMeIn connections and access to the product page.
Resources:
  - Link: https://knowledge.broadcom.com/external/article/181241/how-to-block-logmein-with-edge-swg-black.html
Tags:
  - RMM
Acknowledgement:
  - Person:
    Handle:
---