---
title: Create and manage roles for role-based access control
description: Create roles and define the permissions assigned to the role as part of the role-based access control implementation 
keywords: user roles, roles, access rbac
search.product: eADQiWindows 10XVcnh
search.appverid: met150
ms.prod: w10
ms.mktglfcycl: deploy
ms.sitesec: library
ms.pagetype: security
ms.author: macapara
author: mjcaparas
ms.localizationpriority: medium
manager: dansimp
audience: ITPro
ms.collection: M365-security-compliance 
ms.topic: article
---

# Create and manage roles for role-based access control
**Applies to:**

- [Windows Defender Advanced Threat Protection (Windows Defender ATP)](https://go.microsoft.com/fwlink/p/?linkid=2069559)


>Want to experience Windows Defender ATP? [Sign up for a free trial.](https://www.microsoft.com/en-us/WindowsForBusiness/windows-atp?ocid=docs-wdatp-roles-abovefoldlink)

## Create roles and assign the role to an Azure Active Directory group
The following steps guide you on how to create roles in Windows Defender Security Center. It assumes that you have already created Azure Active Directory user groups.

1.	In the navigation pane, select **Settings > Roles**.

2.	Click **Add role**. 

3.	Enter the role name, description, and permissions you'd like to assign to the role.

	 - **Role name**
	 - **Description**
	 - **Permissions**
		  - **View data** - Users can view information in the portal.
		  - **Alerts investigation** - Users can manage alerts, initiate automated investigations, collect investigation packages, manage machine tags, and export machine timeline.
		  - **Active remediation actions** - Users can take response actions and approve or dismiss pending remediation actions.
          - **Manage portal system settings** - Users can configure storage settings, SIEM and threat intel API settings (applies globally), advanced settings, automated file uploads, roles and machine groups.
            
            >[!NOTE]
            >This setting is only available in the Windows Defender ATP administrator (default) role. 

		  - **Manage security settings** - Users can configure alert suppression settings, manage allowed/blocked lists for automation, manage folder exclusions for automation, onboard and offboard machines, and manage email notifications.
		  
4.	Click **Next** to assign the role to an Azure AD group.

5.	Use the filter to select the Azure AD group that you'd like to add to this role.

6.	Click **Save and close**.

7.	Apply the configuration settings.


After creating roles, you'll need to create a machine group and provide access to the machine group by assigning it to a role that you just created. 

>[!NOTE]
>The Windows Defender ATP administrator (default) role has administrator permissions. Administrator permissions cannot be assigned to any other role. Only those who are assigned the Windows Defender ATP administrator role, has access to all machine groups.

## Edit roles

1.	Select the role you'd like to edit.

2.	Click **Edit**.

3.	Modify the details or the groups that are assigned to the role. 

4.	Click **Save and close**.

## Delete roles

1.	Select the role you'd like to delete.

2.	Click the drop-down button and select **Delete role**.


##Related topics
- [User basic permissions to access the portal](basic-permissions-windows-defender-advanced-threat-protection.md)
- [Create and manage machine groups](machine-groups-windows-defender-advanced-threat-protection.md)
