------------------------------------------------------------
ENTERPRISE WINDOWS INFRASTRUCTURE LAB
------------------------------------------------------------


------------------------------------------------------------
PROJECT OVERVIEW
------------------------------------------------------------

This project documents the design, deployment, and administration
of a simulated enterprise Windows infrastructure environment for
Kojay Industries.


## BUSINESS SCENARIO

Kojay Industries is a growing organization that requires a
centralized IT infrastructure for user authentication, device
management, internal name resolution, file access, and corporate
policy enforcement.

The environment will begin with a central corporate Active Directory
infrastructure and a Calgary site. As the organization grows, the
environment will be expanded to support additional users, services,
administrative requirements, and geographic locations such as
Toronto and Edmonton.

------------------------------------------------------------
PROJECT GOALS
------------------------------------------------------------

- Deploy and administer Windows Server infrastructure
- Configure Active Directory Domain Services
- Configure and manage DNS
- Create and manage users, groups, and organizational units
- Automate administrative tasks using PowerShell
- Configure Group Policy
- Deploy centralized file services
- Manage NTFS and share permissions
- Design and administer multi-site Active Directory infrastructure
- Implement delegated administration and least privilege
- Configure backup and recovery
- Integrate Linux infrastructure
- Implement infrastructure monitoring


## INITIAL ENVIRONMENT

- Company: Kojay Industries
- Active Directory Domain: corp.kojayindustries.test
- Initial Site: Calgary
- Network: 10.10.10.0/24  

Systems:
- KI-CORP-DC01 - Windows Server 2025, Initial Corporate Domain Controller / DNS
- KI-CGY-DC01 - Windows Server 2025, Calgary Site Domain Controller / DNS
- KI-CGY-LNX01 - CentOS 10, Linux Infrastructure Server
- KI-CGY-CL01 - Windows 11 Pro, Calgary Domain Workstation


------------------------------------------------------------
INFRASTRUCTURE DIAGRAM
------------------------------------------------------------
Infrastructure diagram will be updated as the environment is built.


------------------------------------------------------------
PROJECT STAGES
------------------------------------------------------------

Stage 01 - Core Active Directory Infrastructure
Stage 02 - Active Directory Organization and User Automation
Stage 03 - File Services and Group Policy
Stage 04 - Multi-Site Active Directory Expansion
Stage 05 - Secure Administration and Recovery
Stage 06 - Infrastructure Monitoring and Validation


------------------------------------------------------------
TECHNOLOGIES
------------------------------------------------------------
- VMware Workstation
- Windows Server 2025
- Windows 11 Pro
- CentOS 10
- Active Directory Domain Services
- DNS
- PowerShell
- Group Policy
- SMB
- NTFS Permissions
- Active Directory Sites and Services
- TCP/IP


------------------------------------------------------------
DOCUMENTATION APPROACH
------------------------------------------------------------

Each stage of the project represents a new business or
infrastructure requirement for Kojay Industries.

Each stage will document:
- Business Scenario
- Objective
- Environment Changes
- Design Decisions
- Implementation
- Verification
- Troubleshooting
- Screenshots
- Skills Demonstrated


------------------------------------------------------------
PROJECT STATUS
------------------------------------------------------------

- Stage 01 - In Progress
- Stage 02 - Planned
- Stage 03 - Planned
- Stage 04 - Planned
- Stage 05 - Planned
- Stage 06 - Planned

