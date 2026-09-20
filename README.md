## Group 9 Documentation ## 
Minh Ly, Kenny Yang, Ivan Shao 

<img width="806" height="259" alt="Topology (1)" src="https://github.com/user-attachments/assets/3ed24318-4b36-49c9-9cb3-23a666042ae1" />
# Quick Looks # 
Windows Side: 
  -  Domain:           Windows.Lab
  -  IP Scheme:        192.168.10.xxx

Linux Side: 
  - Domain:            Linux.Lab
  - IP Scheme:         192.168.20.xxx

IP Table: 
  | Device            | IP              | Domain | Interface | 
  |-------------------|-----------------|--------|-----------|
  | pfSense           | 192.168.xxx.254 |        |           |
  | Windows Server    | 192.168.10.2    |        | LAN vmx1  |
  | Linux RHEL Server | 192.168.20.2    |        | OPT1 vmx2 |
  | Linux Client      | 192.168.20.10   |        | OPT1 vmx2 |

  | Service           | Username  | Password |
  |-------------------|-----------|----------|
  | pfSense GUI       | admin     | pfsense  |
  | Windows Server    | student   | student  |
  | Linux RHEL Server | student   | student  |
  | Linux Client      | student   | student  |
  |                   |           |          |

Forward Zones: 


# Lab 1 # 
To Do: 
 - ~~Deploy VM's~~
 - Set up Windows AD
    - ~~Set up DHCP scopes.~~
    - Set up DNS.
 - Set up RHEL AD
    - Download IDM packages.
 - Set up Cross-Realm Trust.
 - ~~Set up DHCP Relay on router.~~
 - Set up Linux Client Integration (SSSD).
 - Set up HBAC Rules, Sudo Delegation, and Advanced Validation. 
