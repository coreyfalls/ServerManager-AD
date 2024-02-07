            +--------------------------------------+
            |         Oracle VirtualBox            |
            |                                      |
            |   +-----------------------------+    |
            |   |   Windows Server 2019      |    |
            |   |    (Virtual Machine)       |    |
            |   +--------------|--------------+    |
            |                  |                  |
            |   +--------------|--------------+    |
            |   |   Active Directory         |    |
            |   |     DNS Server             |    |
            |   +--------------|--------------+    |
            |                  |                  |
            |   +--------------|--------------+    |
            |   |   Windows 10 ISO           |    |
            |   +--------------|--------------+    |
            |                  |                  |
            |   +--------------|--------------+    |
            |   |   Client Machines           |    |
            |   +------------------------------+   |
            +--------------------------------------+


-Oracle VirtualBox hosts the Windows Server 2019 virtual machine.

-The Windows Server 2019 virtual machine runs Active Directory Domain Services (AD DS) and DNS Server roles.

-The Windows 10 ISO is available as a resource.

-Client machines interact with the Active Directory domain for authentication and resource access.




Installation of Windows Server 2019 (ISO):
-------------------------------------
1. Install Windows Server 2019(ISO) on a virtual machine using Oracle VirtualBox. Ensure that the virtual machine meets the minimum system requirements.

Configuration of Basic Server Settings:
----------------------------------------
1. Configure network settings, such as IP address, subnet mask, gateway, and DNS.

Installation of Active Directory Domain Services (AD DS):
---------------------------------------------------------
1. Use the Server Manager to install the Active Directory Domain Services role.
2. Promote the server to a domain controller.

Configuration of Active Directory Domain Services:
---------------------------------------------------
1. Set up the domain name and forest.
2. Specify the domain functional level and forest functional level.

Creation of Organizational Units (OUs):
----------------------------------------
1. Create OUs to organize users, groups, and computers within the domain.

Addition of Users and Groups:
-------------------------------
1. Create user accounts and groups as needed for the network.

Configuration of Group Policies:
---------------------------------
1. Define Group Policy Objects (GPOs) to enforce security settings, desktop configurations, and other policies across the domain.

Additional Resources:
---------------------
- The Windows 10 ISO is added as a resource.
- Client machines (potentially multiple) are included as part of the network, interacting with the Active Directory domain for authentication and resource access.
- The DNS server resolves domain names for both internal and external network communication.

