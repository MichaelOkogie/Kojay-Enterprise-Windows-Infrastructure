# Stage 01 - Core Active Directory Infrastructure

------------------------------------------------------------
BUSINESS SCENARIO
------------------------------------------------------------

Kojay Industries is establishing its first centralized IT
infrastructure at its Calgary headquarters.

As the organization grows, it requires centralized user
authentication, computer management, and internal name resolution. 
Management also requires redundancy so that authentication and
directory services remain available if one domain controller
becomes unavailable.


------------------------------------------------------------
OBJECTIVE
------------------------------------------------------------

Deploy the initial Kojay Industries Active Directory environment
using two Windows Server 2025 domain controllers, one Ubuntu Server,
and one Windows 11 Pro workstation.

This stage will establish the corporate domain, configure DNS,
introduce domain controller redundancy, and verify that the first
corporate workstation can successfully authenticate to the domain.


------------------------------------------------------------
ENVIRONMENT
------------------------------------------------------------

- Company: Kojay Industries
- Primary Site: Calgary
- Active Directory Domain: corp.kojayindustries.test
- Network:
- 10.10.10.0/24 
  
Systems:  

KI-CGY-DC01
- Windows Server 2025
- Primary Domain Controller
- DNS Server
- IP: 10.10.10.10 

KI-CGY-DC02
- Windows Server 2025
- Additional Domain Controller
- DNS Server
- IP: 10.10.10.11 

KI-CGY-LNX01
- Ubuntu Server
- Linux Infrastructure Server
- IP: 10.10.10.20 

KI-CGY-CL01
- Windows 11 Pro
- Domain Workstation
- IP: 10.10.10.100 


------------------------------------------------------------
NAMING CONVENTION
------------------------------------------------------------

The following naming structure is used throughout the environment: \

KI-[SITE]-[ROLE][NUMBER]
\
Example:
KI-CGY-DC01
KI  = Kojay Industries
CGY = Calgary
DC  = Domain Controller
01  = Device Number


------------------------------------------------------------
IP ADDRESSING PLAN
------------------------------------------------------------

Calgary Network:
10.10.10.0/24

Gateway:
10.10.10.1

Reserved Infrastructure:

10.10.10.10 - 10.10.10.19
Domain Controllers

10.10.10.20 - 10.10.10.39
Servers

10.10.10.40 - 10.10.10.49
Network Infrastructure

10.10.10.100 - 10.10.10.199
Client Workstations


------------------------------------------------------------
IMPLEMENTATION PLAN
------------------------------------------------------------

1. Create the four virtual machines in VMware Workstation.

2. Configure the Calgary virtual network.

3. Rename each system according to the Kojay Industries naming
   convention.

4. Assign static IP addresses to the servers.

5. Install Active Directory Domain Services and DNS on KI-CGY-DC01.

6. Create the corp.kojayindustries.test forest and domain.

7. Join KI-CGY-DC02 to the domain.

8. Promote KI-CGY-DC02 as an additional domain controller and
   DNS server.

9. Verify Active Directory replication between both domain
   controllers.

10. Verify DNS resolution.

11. Join KI-CGY-CL01 to the domain.

12. Create a test domain user.

13. Sign in to KI-CGY-CL01 using the domain account.

14. Verify domain authentication, DNS resolution, and replication.


------------------------------------------------------------
VERIFICATION
------------------------------------------------------------

The following will be used to verify successful implementation:

- Both domain controllers appear in Active Directory.
- DNS records are available and name resolution is functional.
- Active Directory replication completes successfully.
- KI-CGY-CL01 successfully joins the domain.
- A domain user can authenticate on KI-CGY-CL01.
- Systems can resolve each other using hostnames.
- KI-CGY-DC02 can provide directory and DNS services if required.


------------------------------------------------------------
SCREENSHOTS
------------------------------------------------------------

Screenshots captured during this stage will demonstrate:

- VMware virtual machine environment
- Active Directory Domain Services installation
- Domain creation
- Additional domain controller configuration
- DNS configuration
- Active Directory replication
- Windows 11 domain membership
- Successful domain user authentication


------------------------------------------------------------
TROUBLESHOOTING
------------------------------------------------------------

Any configuration issues encountered during implementation will
be documented here, including:

- Symptoms
- Cause
- Troubleshooting steps
- Resolution


------------------------------------------------------------
SKILLS DEMONSTRATED
------------------------------------------------------------

- VMware Workstation
- Windows Server 2025
- Active Directory Domain Services
- DNS
- Domain Controller Deployment
- Active Directory Replication
- TCP/IP Configuration
- Windows Domain Membership
- User Authentication
- Windows Systems Administration
