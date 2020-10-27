(Deprecated) Stop all Azure VMs (ARM and ASM) in a subscription
===============================================================

            

**Updated at 05/17/2019 : This runbook is deprecated. You should use the new Az Powershell module by using [this runbook to stop / start VMs in parallel](https://gallery.technet.microsoft.com/scriptcenter/Stop-Start-all-or-only-8a7e11a2?redir=0) or [this runbook to stop /start VMs in sequence](https://gallery.technet.microsoft.com/scriptcenter/Az-Stop-Start-all-or-only-8a8fcab4?redir=0). **


**[See more about the new **Az PowerShell module for Azure**](https://docs.microsoft.com/en-us/powershell/azure/new-azureps-module-az?view=azps-2.0.0)**


This runbook connects to Azure and stops all VMs (ASM and ARM) in the specified Azure subscription. You can attach a schedule to this runbook to run it at a specific time.


**Updated at 02/24/2016 : **Bug fixed when selecting Azure subscription and working against classic virtual machines.


**Requirements**


1. An Automation variable asset called 'AzureSubscriptionId' that contains the GUID for this Azure subscription.  To use an asset with a different name you can pass the asset name as a runbook input parameter or change the default value for the input
 parameter. 


2. An Automation credential asset called 'AzureCred' that contains the Azure AD user credential with authorization for this subscription.  To use an asset with a different name you can pass the asset name as a runbook input parameter or change the default
 value for the input parameter.


3. Version 1.0.3 or higher of all Azure modules in your Azure Automation account. This runbook uses the Get-AzureRmResourceGroup cmdlet available in the version 1.0.3 of AzureRM.Resources module.


**Runbook content**


 

 

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
