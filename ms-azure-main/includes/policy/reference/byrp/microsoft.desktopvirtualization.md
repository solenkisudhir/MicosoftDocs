---
author: davidsmatlak
ms.service: azure-policy
ms.topic: include
ms.date: 01/02/2024
ms.author: davidsmatlak
ms.custom: generated
---

|Name<br /><sub>(Azure portal)</sub> |Description |Effect(s) |Version<br /><sub>(GitHub)</sub> |
|---|---|---|---|
|[Azure Virtual Desktop hostpools should disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fc25dcf31-878f-4eba-98eb-0818fdc6a334) |Disabling public network access improves security and keeps your data safe by ensuring that access to the Azure Virtual Desktop service is not exposed to the public internet. Learn more at: [https://aka.ms/avdprivatelink](https://aka.ms/avdprivatelink). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Desktop%20Virtualization/DesktopVirtualizationHostpool_PrivateNetworkOnly_AuditDeny.json) |
|[Azure Virtual Desktop hostpools should disable public network access only on session hosts](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fa22065a3-3b04-46ff-b84c-2d30e5c300d0) |Disabling public network access for your Azure Virtual Desktop hostpool session hosts, but allowing public access for end users improves security by limiting exposure to the public internet. Learn more at: [https://aka.ms/avdprivatelink](https://aka.ms/avdprivatelink). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Desktop%20Virtualization/DVHostpool_PrivateNetworkPublicClient_AuditDeny.json) |
|[Azure Virtual Desktop service should use private link](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fca950cd7-02f7-422e-8c23-91ff40f169c1) |Using Azure Private Link with your Azure Virtual Desktop resources can improve security and keep your data safe. Learn more about private links at: [https://aka.ms/avdprivatelink](https://aka.ms/avdprivatelink). |Audit, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Desktop%20Virtualization/DesktopVirtualization_PrivateEndpoint_Audit.json) |
|[Azure Virtual Desktop workspaces should disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F87ac3038-c07a-4b92-860d-29e270a4f3cd) |Disabling public network access for your Azure Virtual Desktop workspace resource prevents the feed from being accessible over the public internet. Allowing only private network access improves security and keeps your data safe. Learn more at: [https://aka.ms/avdprivatelink](https://aka.ms/avdprivatelink). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Desktop%20Virtualization/DVWorkspace_PrivateNetworkAccess_AuditDeny.json) |
|[Configure Azure Virtual Desktop hostpools to disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F2a0913ff-51e7-47b8-97bb-ea17127f7c8d) |Disable public network access for session hosts and end users on your Azure Virtual Desktop hostpool resource so that it's not accessible over the public internet. This improves security and keeps your data safe. Learn more at: [https://aka.ms/avdprivatelink](https://aka.ms/avdprivatelink). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Desktop%20Virtualization/DesktopVirtualizationHostpool_PrivateNetworkOnly_Modify.json) |
|[Configure Azure Virtual Desktop hostpools to disable public network access only for session hosts](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fe84e8a9a-f43e-46e3-9458-bbcfb2d7e429) |Disable public network access for your Azure Virtual Desktop hostpool session hosts, but allow public access for end users. This allows users to still access AVD service while ensuring the session host is only accessible through private routes. Learn more at: [https://aka.ms/avdprivatelink](https://aka.ms/avdprivatelink). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Desktop%20Virtualization/DVHostpool_PrivateNetworkPublicClient_Modify.json) |
|[Configure Azure Virtual Desktop hostpools with private endpoints](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F7b331e6b-6096-4395-a754-758a64505f19) |Private endpoints connect your virtual network to Azure services without a public IP address at the source or destination. By mapping private endpoints to your Azure Virtual Desktop resources, you can improve security and keep your data safe. Learn more at: [https://aka.ms/avdprivatelink](https://aka.ms/avdprivatelink). |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Desktop%20Virtualization/DVHostpool_PrivateEndpoint_DINE.json) |
|[Configure Azure Virtual Desktop workspaces to disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fce6ebf1d-0b94-4df9-9257-d8cacc238b4f) |Disable public network access for your Azure Virtual Desktop workspace resource so the feed is not accessible over the public internet. This improves security and keeps your data safe. Learn more at: [https://aka.ms/avdprivatelink](https://aka.ms/avdprivatelink). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Desktop%20Virtualization/DesktopVirtualizationWorkspace_PrivateNetworkAccess_Modify.json) |
|[Configure Azure Virtual Desktop workspaces with private endpoints](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F02aa841c-42e8-492f-a43d-1f2c67e58d41) |Private endpoints connect your virtual network to Azure services without a public IP address at the source or destination. By mapping private endpoints to your Azure Virtual Desktop resources, you can improve security and keep your data safe. Learn more at: [https://aka.ms/avdprivatelink](https://aka.ms/avdprivatelink). |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Desktop%20Virtualization/DVWorkspace_PrivateEndpoint_DINE.json) |