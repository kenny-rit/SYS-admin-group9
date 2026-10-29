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
  | Graylog           | 192.168.20.14   |        |           |
  | Zabbix            | 192.168.20.15   |        |           |

  | Service           | Username  | Password |
  |-------------------|-----------|----------|
  | pfSense GUI       | admin     | pfsense  |
  | Windows Server    | student   | student  |
  | Linux RHEL Server | student   | student  |
  | Linux Client      | student   | student  |
  | Graylog           | student   | student  | 
  | Zabbix            | student   | student  |

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

# Lab 2 #
 - Update github.

# Lab 3 # 

 - Provision Storage & Automation Hosts
   - Deploy TrueNAS SCALE VM with dedicated boot and data disks
   - Provision Rocky Linux VM for Cronicle
   - Configure DNS A/PTR records for both hosts


 - Configure ZFS Storage Infrastructure
   - Set up redundant ZFS pool (`tank`) using a 2-disk mirror
   - Create child datasets separated by purpose (SMB, NFS, Backup)


 - Integrate Directory Services & Implement File Shares
   - Join TrueNAS to Active Directory
   - Configure SMB share with group-based ACLs (Writer vs. Reader access)
   - Export NFS share and mount on Rocky Linux client (including `/etc/fstab` persistence)


 - Implement Data Protection & Recovery
   - Configure periodic ZFS snapshot tasks
   - Set up local snapshot replication tasks
   - Perform and verify file recovery from a snapshot


 - Deploy Automation & System Observability
   - Install Node.js 22.x and deploy Cronicle scheduler
   - Create and execute a storage/share health validation job in Cronicle
   - Integrate TrueNAS with observability stack (Zabbix host or Graylog log monitoring)


 - Complete Lab Documentation & Reflection
   - Update architecture diagram and record troubleshooting entries / contributions
   - Complete required figures (1–10) and answer reflection questions (Q1–Q5)
