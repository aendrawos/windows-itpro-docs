---
title: Configuring Hybrid Azure AD joined key trust Windows Hello for Business - Active Directory (AD)
description: Configuring Hybrid key trust Windows Hello for Business - Active Directory (AD)
ms.date: 4/30/2021
appliesto: 
- ✅ <a href=https://learn.microsoft.com/windows/release-health/supported-versions-windows-client target=_blank>Windows 10 and later</a>
ms.topic: article
---
# Configuring Hybrid Azure AD joined key trust Windows Hello for Business: Active Directory

[!INCLUDE [hello-hybrid-key-trust](../../includes/hello-hybrid-key-trust-ad.md)]

Configure the appropriate security groups to efficiently deploy Windows Hello for Business to users. 

### Creating Security Groups

Windows Hello for Business uses a security group to simplify the deployment and management.

#### Create the Windows Hello for Business Users Security Group

The Windows Hello for Business Users group is used to make it easy to deploy Windows Hello for Business in phases.  You assign Group Policy and Certificate template permissions to this group to simplify the deployment by simply adding the users to the group.  This provides users with the proper permissions to provision Windows Hello for Business and to enroll in the Windows Hello for Business authentication certificate.

Sign-in a domain controller or management workstation with *Domain Admin* equivalent credentials.

1. Open **Active Directory Users and Computers**.
2. Click **View** and click **Advanced Features**.
3. Expand the domain node from the navigation pane.
4. Right-click the **Users** container. Click **New**. Click **Group**.
5. Type **Windows Hello for Business Users** in the **Group Name** text box.
6. Click **OK**.

### Section Review

> [!div class="checklist"]
> * Create the Windows Hello for Business Users group
> 
> [!div class="step-by-step"]
> [< Configure Windows Hello for Business](hello-hybrid-key-whfb-settings.md)
> [Configure Azure AD Connect >](hello-hybrid-key-whfb-settings-dir-sync.md)

<br><br>

<hr>

## Follow the Windows Hello for Business hybrid key trust deployment guide

1. [Overview](hello-hybrid-cert-trust.md)
2. [Prerequisites](hello-hybrid-key-trust-prereqs.md)
3. [New Installation Baseline](hello-hybrid-key-new-install.md)
4. [Configure Directory Synchronization](hello-hybrid-key-trust-dirsync.md)
5. [Configure Azure Device Registration](hello-hybrid-key-trust-devreg.md)
6. Configure Windows Hello for Business settings: Active Directory (*You are here*)
7. [Sign-in and Provision](hello-hybrid-key-whfb-provision.md)
