Syncing On-Premises Active Directory to Microsoft Entra ID

Project Overview

This project demonstrates the deployment of a hybrid identity environment by integrating an on-premises Active Directory Domain Services (AD DS) environment with Microsoft Entra ID using Microsoft Entra Connect Sync.

The objective was to understand how organizations synchronize identities between on-premises infrastructure and cloud environments while maintaining centralized identity management.

Technologies Used

* Windows Server
* Active Directory Domain Services (AD DS)
* Microsoft Entra ID
* Microsoft Entra Connect Sync
* Organizational Units (OUs)
* User and Group Management
* Hybrid Identity


Project Architecture

On-Premises Active Directory

↓

Microsoft Entra Connect Sync

↓

Microsoft Entra ID


Implementation Steps

1. Deploy Windows Server

A Windows Server virtual machine was deployed to serve as the domain controller.

2. Install Active Directory Domain Services

The AD DS role was installed together with the required management tools and dependencies.

3. Promote the Server to a Domain Controller

A new forest was created and the server was promoted to become the first domain controller in the environment.

4. Create Organizational Units and Test Users

Several Organizational Units (OUs) and test user accounts were created to simulate a typical enterprise environment.

5. Configure Microsoft Entra Connect

Microsoft Entra Connect Sync was downloaded and installed.

The Express Settings deployment option was used to:

* Configure synchronization services
* Enable Password Hash Synchronization
* Configure Microsoft Entra ID connectivity
* Configure Active Directory connectivity

6. Verify Synchronization

After configuration completed successfully, user objects were synchronized from Active Directory to Microsoft Entra ID.


Key Lessons Learned

* Hybrid identity remains critical in many enterprise environments.
* Identity synchronization simplifies administration across cloud and on-premises environments.
* Understanding the identity lifecycle is essential for cloud and security professionals.
* Microsoft Entra Connect provides a straightforward way to bridge Active Directory and Microsoft Entra ID.
* Identity is increasingly becoming the primary security boundary in modern organizations.



Related Article

I documented the full project experience in a Medium article:

Why Hybrid Identity Still Matters in a Cloud-First World

Medium Profile:
https://medium.com/@tegaaruvwe

Author

Tega Avwaghwaruvwe

Cloud Engineer | Microsoft Entra ID | Azure Security | Identity & Access Management (IAM) | Cloud Security

GitHub: https://github.com/tegs3