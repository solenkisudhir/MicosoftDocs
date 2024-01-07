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
|[Configure container registries to disable anonymous authentication.](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fcced2946-b08a-44fe-9fd9-e4ed8a779897) |Disable anonymous pull for your registry so that data not accessible by unauthenticated user. Disabling local authentication methods like admin user, repository scoped access tokens and anonymous pull improves security by ensuring that container registries exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/acr/authentication](https://aka.ms/acr/authentication). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_AnonymousPullDisabled_Modify.json) |
|[Configure container registries to disable ARM audience token authentication.](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F785596ed-054f-41bc-aaec-7f3d0ba05725) |Disable Azure Active Directory ARM audience tokens for authentication to your registry. Only Azure Container Registry (ACR) audience tokens will be used for authentication. This will ensure only tokens meant for usage on the registry can be used for authentication. Disabling ARM audience tokens does not affect admin user's or scoped access tokens' authentication. Learn more at: [https://aka.ms/acr/authentication](https://aka.ms/acr/authentication). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_AADAuthenticationAsArmDisabled_Modify.json) |
|[Configure container registries to disable local admin account.](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F79fdfe03-ffcb-4e55-b4d0-b925b8241759) |Disable admin account for your registry so that it is not accessible by local admin. Disabling local authentication methods like admin user, repository scoped access tokens and anonymous pull improves security by ensuring that container registries exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/acr/authentication](https://aka.ms/acr/authentication). |Modify, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_AdminAccountDisabled_Modify.json) |
|[Configure Container registries to disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fa3701552-92ea-433e-9d17-33b7f1208fc9) |Disable public network access for your Container Registry resource so that it's not accessible over the public internet. This can reduce data leakage risks. Learn more at [https://aka.ms/acr/portal/public-network](https://aka.ms/acr/portal/public-network) and [https://aka.ms/acr/private-link](https://aka.ms/acr/private-link). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_PublicNetworkAccess_Modify.json) |
|[Configure container registries to disable repository scoped access token.](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fa9b426fe-8856-4945-8600-18c5dd1cca2a) |Disable repository scoped access tokens for your registry so that repositories are not accessible by tokens. Disabling local authentication methods like admin user, repository scoped access tokens and anonymous pull improves security by ensuring that container registries exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/acr/authentication](https://aka.ms/acr/authentication). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_TokenDisabled_Modify.json) |
|[Configure Container registries to use private DNS zones](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fe9585a95-5b8c-4d03-b193-dc7eb5ac4c32) |Use private DNS zones to override the DNS resolution for a private endpoint. A private DNS zone links to your virtual network to resolve to your Container Registry. Learn more at: [https://aka.ms/privatednszone](https://aka.ms/privatednszone) and [https://aka.ms/acr/private-link](https://aka.ms/acr/private-link). |DeployIfNotExists, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_PrivateDNSZone_DeployIfNotExists.json) |
|[Configure Container registries with private endpoints](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fd85c6833-7d33-4cf5-a915-aaa2de84405f) |Private endpoints connect your virtual network to Azure services without a public IP address at the source or destination. By mapping private endpoints to your premium container registry resources, you can reduce data leakage risks. Learn more at: [https://aka.ms/privateendpoints](https://aka.ms/privateendpoints) and [https://aka.ms/acr/private-link](https://aka.ms/acr/private-link). |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_PrivateEndpoint_DeployIfNotExists.json) |
|[Container registries should be encrypted with a customer-managed key](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F5b9159ae-1701-4a6f-9a7a-aa9c8ddd0580) |Use customer-managed keys to manage the encryption at rest of the contents of your registries. By default, the data is encrypted at rest with service-managed keys, but customer-managed keys are commonly required to meet regulatory compliance standards. Customer-managed keys enable the data to be encrypted with an Azure Key Vault key created and owned by you. You have full control and responsibility for the key lifecycle, including rotation and management. Learn more at [https://aka.ms/acr/CMK](https://aka.ms/acr/CMK). |Audit, Deny, Disabled |[1.1.2](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_CMKEncryptionEnabled_Audit.json) |
|[Container registries should have anonymous authentication disabled.](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F9f2dea28-e834-476c-99c5-3507b4728395) |Disable anonymous pull for your registry so that data is not accessible by unauthenticated user. Disabling local authentication methods like admin user, repository scoped access tokens and anonymous pull improves security by ensuring that container registries exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/acr/authentication](https://aka.ms/acr/authentication). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_AnonymousPullDisabled_AuditDeny.json) |
|[Container registries should have ARM audience token authentication disabled.](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F42781ec6-6127-4c30-bdfa-fb423a0047d3) |Disable Azure Active Directory ARM audience tokens for authentication to your registry. Only Azure Container Registry (ACR) audience tokens will be used for authentication. This will ensure only tokens meant for usage on the registry can be used for authentication. Disabling ARM audience tokens does not affect admin user's or scoped access tokens' authentication. Learn more at: [https://aka.ms/acr/authentication](https://aka.ms/acr/authentication). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_AADAuthenticationAsArmPolicy_AuditDeny.json) |
|[Container registries should have exports disabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F524b0254-c285-4903-bee6-bb8126cde579) |Disabling exports improves security by ensuring data in a registry is accessed solely via the dataplane ('docker pull'). Data cannot be moved out of the registry via 'acr import' or via 'acr transfer'. In order to disable exports, public network access must be disabled. Learn more at: [https://aka.ms/acr/export-policy](https://aka.ms/acr/export-policy). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_ExportPolicy_AuditDeny.json) |
|[Container registries should have local admin account disabled.](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fdc921057-6b28-4fbe-9b83-f7bec05db6c2) |Disable admin account for your registry so that it is not accessible by local admin. Disabling local authentication methods like admin user, repository scoped access tokens and anonymous pull improves security by ensuring that container registries exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/acr/authentication](https://aka.ms/acr/authentication). |Audit, Deny, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_AdminAccountDisabled_AuditDeny.json) |
|[Container registries should have repository scoped access token disabled.](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fff05e24e-195c-447e-b322-5e90c9f9f366) |Disable repository scoped access tokens for your registry so that repositories are not accessible by tokens. Disabling local authentication methods like admin user, repository scoped access tokens and anonymous pull improves security by ensuring that container registries exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/acr/authentication](https://aka.ms/acr/authentication). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_TokenDisabled_AuditDeny.json) |
|[Container registries should have SKUs that support Private Links](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fbd560fc0-3c69-498a-ae9f-aa8eb7de0e13) |Azure Private Link lets you connect your virtual network to Azure services without a public IP address at the source or destination. The private link platform handles the connectivity between the consumer and services over the Azure backbone network. By mapping private endpoints to your container registries instead of the entire service, data leakage risks are reduced. Learn more at: [https://aka.ms/acr/private-link](https://aka.ms/acr/private-link). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_SkuSupportsPrivateEndpoints_AuditDeny.json) |
|[Container registries should not allow unrestricted network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fd0793b48-0edc-4296-a390-4c75d1bdfd71) |Azure container registries by default accept connections over the internet from hosts on any network. To protect your registries from potential threats, allow access from only specific private endpoints, public IP addresses or address ranges. If your registry doesn't have network rules configured, it will appear in the unhealthy resources. Learn more about Container Registry network rules here: [https://aka.ms/acr/privatelink,](https://aka.ms/acr/privatelink,) [https://aka.ms/acr/portal/public-network](https://aka.ms/acr/portal/public-network) and [https://aka.ms/acr/vnet](https://aka.ms/acr/vnet). |Audit, Deny, Disabled |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_NetworkRulesExist_AuditDeny.json) |
|[Container registries should prevent cache rule creation](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F84497762-32b6-4ab3-80b6-732ea48b85a2) |Disable cache rule creation for your Azure Container Registry to prevent pull through cache pulls. Learn more at: [https://aka.ms/acr/cache](https://aka.ms/acr/cache). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_PTCDisabled_AuditDeny.json) |
|[Container registries should use private link](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fe8eef0a8-67cf-4eb4-9386-14b0e78733d4) |Azure Private Link lets you connect your virtual network to Azure services without a public IP address at the source or destination. The private link platform handles the connectivity between the consumer and services over the Azure backbone network.By mapping private endpoints to your container registries instead of the entire service, you'll also be protected against data leakage risks. Learn more at: [https://aka.ms/acr/private-link](https://aka.ms/acr/private-link). |Audit, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_PrivateEndpointEnabled_Audit.json) |
|[Public network access should be disabled for Container registries](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F0fdf0491-d080-4575-b627-ad0e843cba0f) |Disabling public network access improves security by ensuring that container registries are not exposed on the public internet. Creating private endpoints can limit exposure of container registry resources. Learn more at: [https://aka.ms/acr/portal/public-network](https://aka.ms/acr/portal/public-network) and [https://aka.ms/acr/private-link](https://aka.ms/acr/private-link). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Container%20Registry/ACR_PublicNetworkAccess_AuditDeny.json) |