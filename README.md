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
 
Lab prerequisites
 
Basic Azure resources used were Subnets, Virtual Machines, Network Security Group (NSG).
 
## Enabling Microsoft Defender for Cloud
Microsoft Defender for Cloud for the standard tier can be enabled on the Workload protections of the Cloud Security pane as shown in the picture below.
