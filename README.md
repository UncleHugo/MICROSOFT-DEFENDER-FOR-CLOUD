# MICROSOFT-DEFENDER-FOR-CLOUD

## Securing your cloud with Microsoft Defender for Cloud

Microsoft Defender for Cloud (previously Azure Security Center) allows you to understand the security state of your cloud resources, as well as your on-premises virtual machines via the Microsoft Monitoring Agent. Microsoft Defender for Cloud is included on all Azure subscriptions at the free service tier. Virtual machines and App Services are the types of resources included in the free tier while many more are available in the standard tier including SQL Databases and Azure Kubernetes Services. Microsoft Defender for Cloud has over 150 rules built-in. With Microsoft Defender for Cloud, you can:

- Understand the security state of all your Azure subscriptions
- Find and fix vulnerable resources and configurations
- Easily deploy and monitor security solutions from partners
- Detect active threats early and respond fast (standard tier only)
- Integrate with your existing security processes and tools
 
For an overview about Microsoft Defender for Cloud Microsoft Defender for Cloud https://learn.microsoft.com/en-us/azure/defender-for-cloud/defender-for-cloud-introduction
 
 
In this lab, I will be enabling Microsoft Defender for Cloud and also show how it can be used to automatically identify security risks that are enabled in the default Microsoft Defender for Cloud security policy. This lab step will give an overview of the recommendations feature of Microsoft Defender for Cloud.

![Architecture](https://github.com/user-attachments/assets/f2f5c6e9-67aa-46a3-9692-cd2a9c77a114)

 
#### Lab prerequisites:
 
Basic Azure resources used were Subnets, Virtual Machines, Network Security Group (NSG), Storage Account
 
## Enabling Microsoft Defender for Cloud
Microsoft Defender for Cloud for the standard tier can be enabled on the Workload protections of the Cloud Security pane as shown in the picture below.

![enablingdefenderforcloud](https://github.com/user-attachments/assets/654905ca-6fe8-44d3-9d8a-5c7040eea225)

![enablingservers](https://github.com/user-attachments/assets/f28a6522-7036-42ba-a4c6-7db26c944702)

Microsoft Defender for Cloud provides comprehensive, cloud-native protections from development to runtime in multi-cloud environments. Workload involving Servers, App Service, Databases, Storage, Containers, AI Services, Key Vault, Resource Manager, APIs can be enabled on the Defender plans in the Environment Settings  under the Management section as shown below.

![environmental](https://github.com/user-attachments/assets/b6fb9013-418f-47c4-a7d9-578932950089)


![defenderplan](https://github.com/user-attachments/assets/ca9a6871-6127-43da-a809-b78b4cfe402a)


## Understanding Microsoft Defender for Cloud recommendations.

In this lab step, i will show how Microsoft Defender for Cloud can be used to automatically identify security risks that are enabled in the default Microsoft Defender for Cloud security policy. This lab step will give an overview of the recommendations feature of Microsoft Defender for Cloud. Under the Recommendations blade in the menu, under the General section:

![recommendation](https://github.com/user-attachments/assets/a56474fb-914f-4e9c-9bc1-fc1474fdbe35)

Clicking on the first recommendation *Virtual machines and virtual machine scale sets should have encryption at host enabled* 
The following page appears after clicking on the recommendation:

![recom2](https://github.com/user-attachments/assets/824730c6-0050-4578-9ffa-dc5038c5d954) 

Reading through the above picture for Description, you can understand that encryption at host is used to get end-to-end encryption for the virtual machine (hugo-vm-1). Encryption at host enables encryption at rest for your temporary disk and OS/data disk caches. Under the Take Action in the picture above, the remediation steps are been provided on how to remediate the issue.
Microsoft Defender for Cloud provides easy-to-follow steps to remedy the risk.

To remediate the issue, following the steps stated below, we navigated to the resource in question which is the (hugo-vm-1) VM

![remediate](https://github.com/user-attachments/assets/c799c64c-b5f7-4106-870f-fd94e44b4470)

![vmsteps](https://github.com/user-attachments/assets/a4af8ce0-71b1-48ac-bd0d-b118c1f71847)

![turn-on](https://github.com/user-attachments/assets/47d9ad6c-88fe-48bb-92a1-c2d4f6a26e6a)

Checking back on the recommendations, we can see in the picture below that the status is marked as COMPLETED

![done](https://github.com/user-attachments/assets/77a39b69-6f42-477d-88a1-22f1e712e280)

Microsoft Defender for Cloud provides a convenient safety net that continues to expand over time, although it should not be treated as a complete security solution. It is advisable to treat Microsoft Defender for Cloud as just one layer of your defense in depth strategy.


## Securing our Storage Account

Going through our storage account *ugoteststorageaccount*, we can see that Microsoft Defender for Cloud (storage) is been turned *on* Fig 12 below

![defender for storage](https://github.com/user-attachments/assets/7d7fc1d4-2213-4879-8e08-87321d972fba)

The fig 13 below shows the recommendations provided by Microsoft Defender for Cloud, it monitors configurations of our storage account for any vulnerabilities and also provides recommendations to mitigate the risk.

![recomstorage](https://github.com/user-attachments/assets/bcafee7f-5c05-41b6-a57a-0f4000b19c00)


![Storageacct](https://github.com/user-attachments/assets/fd7008e4-4d0e-44c3-8811-bc29272e73ad)

![aautofix](https://github.com/user-attachments/assets/a789db15-48f6-4d5b-95b9-fa5af7089a31)

![fixed](https://github.com/user-attachments/assets/437808c2-a858-4c7b-b508-ed715184592f)






























