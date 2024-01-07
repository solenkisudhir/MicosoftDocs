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
|[\[Preview\]: Azure Machine Learning Model Registry Deployments are restricted except for the allowed Registry](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F19539b54-c61e-4196-9a38-67598701be90) |Only deploy Registry Models in the allowed Registry and that are not restricted. |Deny, Disabled |[1.0.0-preview](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/OnlyDeployAllowedRegistryModels_Deny.json) |
|[Azure Machine Learning Compute Instance should have idle shutdown.](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F679ddf89-ab8f-48a5-9029-e76054077449) |Having an idle shutdown schedule reduces cost by shutting down computes that are idle after a pre-determined period of activity. |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/MachineLearningServices_IdleShutdown_Audit.json) |
|[Azure Machine Learning compute instances should be recreated to get the latest software updates](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ff110a506-2dcb-422e-bcea-d533fc8c35e2) |Ensure Azure Machine Learning compute instances run on the latest available operating system. Security is improved and vulnerabilities reduced by running with the latest security patches. For more information, visit [https://aka.ms/azureml-ci-updates/](https://aka.ms/azureml-ci-updates/). |[parameters('effects')] |[1.0.3](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/MachineLearningServices_ComputeInstanceUpdates_Audit.json) |
|[Azure Machine Learning Computes should be in a virtual network](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F7804b5c7-01dc-4723-969b-ae300cc07ff1) |Azure Virtual Networks provide enhanced security and isolation for your Azure Machine Learning Compute Clusters and Instances, as well as subnets, access control policies, and other features to further restrict access. When a compute is configured with a virtual network, it is not publicly addressable and can only be accessed from virtual machines and applications within the virtual network. |Audit, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/MachineLearningServices_Vnet_Audit.json) |
|[Azure Machine Learning Computes should have local authentication methods disabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fe96a9a5f-07ca-471b-9bc5-6a0f33cbd68f) |Disabling local authentication methods improves security by ensuring that Machine Learning Computes require Azure Active Directory identities exclusively for authentication. Learn more at: [https://aka.ms/azure-ml-aad-policy](https://aka.ms/azure-ml-aad-policy). |Audit, Deny, Disabled |[2.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/MachineLearningServices_DisableLocalAuth_Audit.json) |
|[Azure Machine Learning workspaces should be encrypted with a customer-managed key](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fba769a63-b8cc-4b2d-abf6-ac33c7204be8) |Manage encryption at rest of Azure Machine Learning workspace data with customer-managed keys. By default, customer data is encrypted with service-managed keys, but customer-managed keys are commonly required to meet regulatory compliance standards. Customer-managed keys enable the data to be encrypted with an Azure Key Vault key created and owned by you. You have full control and responsibility for the key lifecycle, including rotation and management. Learn more at [https://aka.ms/azureml-workspaces-cmk](https://aka.ms/azureml-workspaces-cmk). |Audit, Deny, Disabled |[1.0.3](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/Workspace_CMKEnabled_Audit.json) |
|[Azure Machine Learning Workspaces should disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F438c38d2-3772-465a-a9cc-7a6666a275ce) |Disabling public network access improves security by ensuring that the Machine Learning Workspaces aren't exposed on the public internet. You can control exposure of your workspaces by creating private endpoints instead. Learn more at: [https://learn.microsoft.com/azure/machine-learning/how-to-configure-private-link?view=azureml-api-2&tabs=azure-portal](../../../../articles/machine-learning/how-to-configure-private-link.md). |Audit, Deny, Disabled |[2.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/Workspace_PublicNetworkAccessDisabled_Audit.json) |
|[Azure Machine Learning workspaces should enable V1LegacyMode to support network isolation backward compatibility](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fe413671a-dd10-4cc1-a943-45b598596cb7) |Azure ML is making a transition to a new V2 API platform on Azure Resource Manager and you can control API platform version using V1LegacyMode parameter. Enabling the V1LegacyMode parameter will enable you to keep your workspaces in the same network isolation as V1, though you won't have use of the new V2 features. We recommend turning on V1 Legacy Mode only when you  want to keep the AzureML control plane data inside your private networks. Learn more at: [https://aka.ms/V1LegacyMode](https://aka.ms/V1LegacyMode). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/Workspace_EnableV1LegacyMode_Audit.json) |
|[Azure Machine Learning workspaces should use private link](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F45e05259-1eb5-4f70-9574-baf73e9d219b) |Azure Private Link lets you connect your virtual network to Azure services without a public IP address at the source or destination. The Private Link platform handles the connectivity between the consumer and services over the Azure backbone network. By mapping private endpoints to Azure Machine Learning workspaces, data leakage risks are reduced. Learn more about private links at: [https://docs.microsoft.com/azure/machine-learning/how-to-configure-private-link](../../../../articles/machine-learning/how-to-configure-private-link.md). |Audit, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/Workspace_PrivateEndpoint_Audit_V2.json) |
|[Azure Machine Learning workspaces should use user-assigned managed identity](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F5f0c7d88-c7de-45b8-ac49-db49e72eaa78) |Manange access to Azure ML workspace and associated resources, Azure Container Registry, KeyVault, Storage, and App Insights using user-assigned managed identity. By default, system-assigned managed identity is used by Azure ML workspace to access the associated resources. User-assigned managed identity allows you to create the identity as an Azure resource and maintain the life cycle of that identity. Learn more at [https://docs.microsoft.com/azure/machine-learning/how-to-use-managed-identities?tabs=python](../../../../articles/machine-learning/how-to-use-managed-identities.md). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/Workspace_UAIEnabled_Audit.json) |
|[Configure Azure Machine Learning Computes to disable local authentication methods](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fa6f9a2d0-cff7-4855-83ad-4cd750666512) |Disable location authentication methods so that your Machine Learning Computes require Azure Active Directory identities exclusively for authentication. Learn more at: [https://aka.ms/azure-ml-aad-policy](https://aka.ms/azure-ml-aad-policy). |Modify, Disabled |[2.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/MachineLearningServices_DisableLocalAuth_Modify.json) |
|[Configure Azure Machine Learning workspace to use private DNS zones](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fee40564d-486e-4f68-a5ca-7a621edae0fb) |Use private DNS zones to override the DNS resolution for a private endpoint. A private DNS zone links to your virtual network to resolve to Azure Machine Learning workspaces. Learn more at: [https://docs.microsoft.com/azure/machine-learning/how-to-network-security-overview](../../../../articles/machine-learning/how-to-network-security-overview.md). |DeployIfNotExists, Disabled |[1.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/Workspace_PrivateDnsZones_DeployIfNotExists.json) |
|[Configure Azure Machine Learning Workspaces to disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fa10ee784-7409-4941-b091-663697637c0f) |Disable public network access for Azure Machine Learning Workspaces so that your workspaces aren't accessible over the public internet. This helps protect the workspaces against data leakage risks. You can control exposure of your workspaces by creating private endpoints instead. Learn more at: [https://learn.microsoft.com/azure/machine-learning/how-to-configure-private-link?view=azureml-api-2&tabs=azure-portal](../../../../articles/machine-learning/how-to-configure-private-link.md). |Modify, Disabled |[1.0.3](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/Workspace_PublicNetworkAccessDisabled_Modify.json) |
|[Configure Azure Machine Learning workspaces with private endpoints](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F7838fd83-5cbb-4b5d-888c-bfa240972597) |Private endpoints connect your virtual network to Azure services without a public IP address at the source or destination. By mapping private endpoints to your Azure Machine Learning workspace, you can reduce data leakage risks. Learn more about private links at: [https://docs.microsoft.com/azure/machine-learning/how-to-configure-private-link](../../../../articles/machine-learning/how-to-configure-private-link.md). |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/Workspace_PrivateEndpoint_DeployIfNotExists.json) |
|[Configure diagnostic settings for Azure Machine Learning Workspaces to Log Analytics workspace](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ff59276f0-5740-4aaf-821d-45d185aa210e) |Deploys the diagnostic settings for Azure Machine Learning Workspaces to stream resource logs to a Log Analytics Workspace when any Azure Machine Learning Workspace which is missing this diagnostic settings is created or updated. |DeployIfNotExists, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/MachineLearningServices_AuditDiagnosticLog_DINE.json) |
|[Resource logs in Azure Machine Learning Workspaces should be enabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fafe0c3be-ba3b-4544-ba52-0c99672a8ad6) |Resource logs enable recreating activity trails to use for investigation purposes when a security incident occurs or when your network is compromised. |AuditIfNotExists, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Machine%20Learning/MachineLearningServices_AuditDiagnosticLog_Audit.json) |