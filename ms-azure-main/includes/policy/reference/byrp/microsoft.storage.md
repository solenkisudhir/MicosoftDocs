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
|[\[Preview\]: Configure backup for blobs on storage accounts with a given tag to an existing backup vault in the same region](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F615b01c4-d565-4f6f-8c6e-d130268e3a1a) |Enforce backup for blobs on all storage accounts that contain a given tag to a central backup vault. Doing this can help you manage backup of blobs contained across multiple storage accounts at scale. For more details, refer to [https://aka.ms/AB-BlobBackupAzPolicies](https://aka.ms/AB-BlobBackupAzPolicies) |DeployIfNotExists, AuditIfNotExists, Disabled |[2.0.0-preview](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Backup/BlobBackupForStorageAccoutsWithTag_Deploy.json) |
|[\[Preview\]: Configure blob backup for all storage accounts that do not contain a given tag to a backup vault in the same region](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F958dbd4e-0e20-4385-a082-d3f20c2a6ad8) |Enforce backup for blobs on all storage accounts that do not contain a given tag to a central backup vault. Doing this can help you manage backup of blobs contained across multiple storage accounts at scale. For more details, refer to [https://aka.ms/AB-BlobBackupAzPolicies](https://aka.ms/AB-BlobBackupAzPolicies) |DeployIfNotExists, AuditIfNotExists, Disabled |[2.0.0-preview](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Backup/BlobBackupForStorageAccoutsWithoutTag_Deploy.json) |
|[\[Preview\]: Storage account public access should be disallowed](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F4fa4b6c0-31ca-4c0d-b10d-24b96f62a751) |Anonymous public read access to containers and blobs in Azure Storage is a convenient way to share data but might present security risks. To prevent data breaches caused by undesired anonymous access, Microsoft recommends preventing public access to a storage account unless your scenario requires it. |audit, Audit, deny, Deny, disabled, Disabled |[3.1.0-preview](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/ASC_Storage_DisallowPublicBlobAccess_Audit.json) |
|[\[Preview\]: Storage Accounts should be Zone Redundant](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F85b005b2-95fc-4953-b9cb-f9ee6427c754) |Storage Accounts can be configured to be Zone Redundant or not. If a Storage Account's SKU name does not end with 'ZRS' or its kind is 'Storage,' it is not Zone Redundant. This policy ensures that your Storage Accounts use ae Zone Redundant configuration. |Audit, Deny, Disabled |[1.0.0-preview](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Resilience/Storage_storageAccounts_ZoneRedundant_Audit.json) |
|[Azure File Sync should use private link](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F1d320205-c6a1-4ac6-873d-46224024e8e2) |Creating a private endpoint for the indicated Storage Sync Service resource allows you to address your Storage Sync Service resource from within the private IP address space of your organization's network, rather than through the internet-accessible public endpoint. Creating a private endpoint by itself does not disable the public endpoint. |AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageSync_PrivateEndpoint_AuditIfNotExists.json) |
|[Configure Azure File Sync with private endpoints](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fb35dddd9-daf7-423b-8375-5a5b86806d5a) |A private endpoint is deployed for the indicated Storage Sync Service resource. This enables you to address your Storage Sync Service resource from within the private IP address space of your organization's network, rather than through the internet-accessible public endpoint. The existence of one or more private endpoints by themselves does not disable the public endpoint. |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageSync_PrivateEndpoint_DeployIfNotExists.json) |
|[Configure diagnostic settings for Blob Services to Log Analytics workspace](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fb4fe1a3b-0715-4c6c-a5ea-ffc33cf823cb) |Deploys the diagnostic settings for Blob Services to stream resource logs to a Log Analytics workspace when any blob Service which is missing this diagnostic settings is created or updated. |DeployIfNotExists, AuditIfNotExists, Disabled |[4.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/BlobServicesLogsToWorkspace_DINE.json) |
|[Configure diagnostic settings for File Services to Log Analytics workspace](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F25a70cc8-2bd4-47f1-90b6-1478e4662c96) |Deploys the diagnostic settings for File Services to stream resource logs to a Log Analytics workspace when any file Service which is missing this diagnostic settings is created or updated. |DeployIfNotExists, AuditIfNotExists, Disabled |[4.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/FileServicesLogsToWorkspace_DINE.json) |
|[Configure diagnostic settings for Queue Services to Log Analytics workspace](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F7bd000e3-37c7-4928-9f31-86c4b77c5c45) |Deploys the diagnostic settings for Queue Services to stream resource logs to a Log Analytics workspace when any queue Service which is missing this diagnostic settings is created or updated. Note: This policy is not triggered upon Storage Account creation and requires creation of a remediation task in order to update for the account. |DeployIfNotExists, AuditIfNotExists, Disabled |[4.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/QueueServicesLogsToWorkspace_DINE.json) |
|[Configure diagnostic settings for Storage Accounts to Log Analytics workspace](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F59759c62-9a22-4cdf-ae64-074495983fef) |Deploys the diagnostic settings for Storage accounts to stream resource logs to a Log Analytics workspace when any storage accounts which is missing this diagnostic settings is created or updated. |DeployIfNotExists, AuditIfNotExists, Disabled |[4.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/AccountStorageLogsToWorkspace_DINE.json) |
|[Configure diagnostic settings for Table Services to Log Analytics workspace](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F2fb86bf3-d221-43d1-96d1-2434af34eaa0) |Deploys the diagnostic settings for Table Services to stream resource logs to a Log Analytics workspace when any table Service which is missing this diagnostic settings is created or updated. Note: This policy is not triggered upon Storage Account creation and requires creation of a remediation task in order to update for the account. |DeployIfNotExists, AuditIfNotExists, Disabled |[4.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/TableServicesLogsToWorkspace_DINE.json) |
|[Configure secure transfer of data on a storage account](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ff81e3117-0093-4b17-8a60-82363134f0eb) |Secure transfer is an option that forces storage account to accept requests only from secure connections (HTTPS). Use of HTTPS ensures authentication between the server and the service and protects data in transit from network layer attacks such as man-in-the-middle, eavesdropping, and session-hijacking |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountSecureTransfer_Modify.json) |
|[Configure Storage account to use a private link connection](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F9f766f00-8d11-464e-80e1-4091d7874074) |Private endpoints connect your virtual network to Azure services without a public IP address at the source or destination. By mapping private endpoints to your storage account, you can reduce data leakage risks. Learn more about private links at - [https://aka.ms/azureprivatelinkoverview](https://aka.ms/azureprivatelinkoverview) |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountPrivateEndpointEnabled_DeployIfNotExists.json) |
|[Configure storage accounts to disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fa06d0189-92e8-4dba-b0c4-08d7669fce7d) |To improve the security of Storage Accounts, ensure that they aren't exposed to the public internet and can only be accessed from a private endpoint. Disable the public network access property as described in [https://aka.ms/storageaccountpublicnetworkaccess](https://aka.ms/storageaccountpublicnetworkaccess). This option disables access from any public address space outside the Azure IP range, and denies all logins that match IP or virtual network-based firewall rules. This reduces data leakage risks. |Modify, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StoragePublicNetworkAccess_Modify.json) |
|[Configure your Storage account public access to be disallowed](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F13502221-8df0-4414-9937-de9c5c4e396b) |Anonymous public read access to containers and blobs in Azure Storage is a convenient way to share data but might present security risks. To prevent data breaches caused by undesired anonymous access, Microsoft recommends preventing public access to a storage account unless your scenario requires it. |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountDisablePublicBlobAccess_Modify.json) |
|[Configure your Storage account to enable blob versioning](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fc36a325b-ae04-4863-ad4f-19c6678f8e08) |You can enable Blob storage versioning to automatically maintain previous versions of an object. When blob versioning is enabled, you can access earlier versions of a blob to recover your data if it's modified or deleted. |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountEnableBlobVersion_Audit.json) |
|[Deploy Defender for Storage (Classic) on storage accounts](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F361c2074-3595-4e5d-8cab-4f21dffc835c) |This policy enables Defender for Storage (Classic) on storage accounts. |DeployIfNotExists, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAdvancedThreatProtection_Deploy.json) |
|[Geo-redundant storage should be enabled for Storage Accounts](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fbf045164-79ba-4215-8f95-f8048dc1780b) |Use geo-redundancy to create highly available applications |Audit, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/GeoRedundant_StorageAccounts_Audit.json) |
|[HPC Cache accounts should use customer-managed key for encryption](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F970f84d8-71b6-4091-9979-ace7e3fb6dbb) |Manage encryption at rest of Azure HPC Cache with customer-managed keys. By default, customer data is encrypted with service-managed keys, but customer-managed keys are commonly required to meet regulatory compliance standards. Customer-managed keys enable the data to be encrypted with an Azure Key Vault key created and owned by you. You have full control and responsibility for the key lifecycle, including rotation and management. |Audit, Disabled, Deny |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageCache_CMKEnabled.json) |
|[Modify - Configure Azure File Sync to disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F0e07b2e9-6cd9-4c40-9ccb-52817b95133b) |The Azure File Sync's internet-accessible public endpoint are disabled by your organizational policy. You may still access the Storage Sync Service via its private endpoint(s). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageSync_IncomingTrafficPolicy_Modify.json) |
|[Modify - Configure your Storage account to enable blob versioning](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F978deb5d-c9a7-41f8-b4b2-b76880d0de1f) |You can enable Blob storage versioning to automatically maintain previous versions of an object. When blob versioning is enabled, you can access earlier versions of a blob to recover your data if it's modified or deleted.  Please note existing storage accounts will not be modified to enable Blob storage versioning. Only newly created storage accounts will have Blob storage versioning enabled |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountEnableBlobVersion_Modify.json) |
|[Public network access should be disabled for Azure File Sync](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F21a8cd35-125e-4d13-b82d-2e19b7208bb7) |Disabling the public endpoint allows you to restrict access to your Storage Sync Service resource to requests destined to approved private endpoints on your organization's network. There is nothing inherently insecure about allowing requests to the public endpoint, however, you may wish to disable it to meet regulatory, legal, or organizational policy requirements. You can disable the public endpoint for a Storage Sync Service by setting the incomingTrafficPolicy of the resource to AllowVirtualNetworksOnly. |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageSync_IncomingTrafficPolicy_AuditDeny.json) |
|[Queue Storage should use customer-managed key for encryption](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ff0e5abd0-2554-4736-b7c0-4ffef23475ef) |Secure your queue storage with greater flexibility using customer-managed keys. When you specify a customer-managed key, that key is used to protect and control access to the key that encrypts your data. Using customer-managed keys provides additional capabilities to control rotation of the key encryption key or cryptographically erase data. |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageQueueCustomerManagedKeyEnabled_Audit.json) |
|[Secure transfer to storage accounts should be enabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F404c3081-a854-4457-ae30-26a93ef643f9) |Audit requirement of Secure transfer in your storage account. Secure transfer is an option that forces your storage account to accept requests only from secure connections (HTTPS). Use of HTTPS ensures authentication between the server and the service and protects data in transit from network layer attacks such as man-in-the-middle, eavesdropping, and session-hijacking |Audit, Deny, Disabled |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/Storage_AuditForHTTPSEnabled_Audit.json) |
|[Storage account containing the container with activity logs must be encrypted with BYOK](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ffbb99e8e-e444-4da0-9ff1-75c92f5a85b2) |This policy audits if the Storage account containing the container with activity logs is encrypted with BYOK. The policy works only if the storage account lies on the same subscription as activity logs by design. More information on Azure Storage encryption at rest can be found here [https://aka.ms/azurestoragebyok](https://aka.ms/azurestoragebyok).  |AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/ActivityLog_StorageAccountBYOK_Audit.json) |
|[Storage account encryption scopes should use customer-managed keys to encrypt data at rest](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fb5ec538c-daa0-4006-8596-35468b9148e8) |Use customer-managed keys to manage the encryption at rest of your storage account encryption scopes. Customer-managed keys enable the data to be encrypted with an Azure key-vault key created and owned by you. You have full control and responsibility for the key lifecycle, including rotation and management. Learn more about storage account encryption scopes at [https://aka.ms/encryption-scopes-overview](https://aka.ms/encryption-scopes-overview). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/Storage_EncryptionScopesShouldUseCMK_Audit.json) |
|[Storage account encryption scopes should use double encryption for data at rest](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fbfecdea6-31c4-4045-ad42-71b9dc87247d) |Enable infrastructure encryption for encryption at rest of your storage account encryption scopes for added security. Infrastructure encryption ensures that your data is encrypted twice. |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageEncryptionScopesShouldUseDoubleEncryption_Audit.json) |
|[Storage account keys should not be expired](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F044985bb-afe1-42cd-8a36-9d5d42424537) |Ensure the user storage account keys are not expired when key expiration policy is set, for improving security of account keys by taking action when the keys are expired. |Audit, Deny, Disabled |[3.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountKeysExpired_Restrict.json) |
|[Storage accounts should allow access from trusted Microsoft services](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fc9d007d0-c057-4772-b18c-01e546713bcd) |Some Microsoft services that interact with storage accounts operate from networks that can't be granted access through network rules. To help this type of service work as intended, allow the set of trusted Microsoft services to bypass the network rules. These services will then use strong authentication to access the storage account. |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccess_TrustedMicrosoftServices_Audit.json) |
|[Storage accounts should be limited by allowed SKUs](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F7433c107-6db4-4ad1-b57a-a76dce0154a1) |Restrict the set of storage account SKUs that your organization can deploy. |Audit, Deny, Disabled |[1.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/AllowedStorageSkus_Audit.json) |
|[Storage accounts should be migrated to new Azure Resource Manager resources](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F37e0d2fe-28a5-43d6-a273-67d37d1f5606) |Use new Azure Resource Manager for your storage accounts to provide security enhancements such as: stronger access control (RBAC), better auditing, Azure Resource Manager based deployment and governance, access to managed identities, access to key vault for secrets, Azure AD-based authentication and support for tags and resource groups for easier security management |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/Classic_AuditForClassicStorages_Audit.json) |
|[Storage accounts should disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fb2982f36-99f2-4db5-8eff-283140c09693) |To improve the security of Storage Accounts, ensure that they aren't exposed to the public internet and can only be accessed from a private endpoint. Disable the public network access property as described in [https://aka.ms/storageaccountpublicnetworkaccess](https://aka.ms/storageaccountpublicnetworkaccess). This option disables access from any public address space outside the Azure IP range, and denies all logins that match IP or virtual network-based firewall rules. This reduces data leakage risks. |Audit, Deny, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StoragePublicNetworkAccess_AuditDeny.json) |
|[Storage accounts should have infrastructure encryption](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F4733ea7b-a883-42fe-8cac-97454c2a9e4a) |Enable infrastructure encryption for higher level of assurance that the data is secure. When infrastructure encryption is enabled, data in a storage account is encrypted twice. |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountInfrastructureEncryptionEnabled_Audit.json) |
|[Storage accounts should have shared access signature (SAS) policies configured](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fbc1b984e-ddae-40cc-801a-050a030e4fbe) |Ensure storage accounts have shared access signature (SAS) expiration policy enabled. Users use a SAS to delegate access to resources in Azure Storage account. And SAS expiration policy recommend upper expiration limit when a user creates a SAS token. |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountSasPolicy_Restrict.json) |
|[Storage accounts should have the specified minimum TLS version](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ffe83a0eb-a853-422d-aac2-1bffd182c5d0) |Configure a minimum TLS version for secure communication between the client application and the storage account. To minimize security risk, the recommended minimum TLS version is the latest released version, which is currently TLS 1.2. |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountMinimumTLSVersion_Audit.json) |
|[Storage accounts should prevent cross tenant object replication](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F92a89a79-6c52-4a7e-a03f-61306fc49312) |Audit restriction of object replication for your storage account. By default, users can configure object replication with a source storage account in one Azure AD tenant and a destination account in a different tenant. It is a security concern because customer's data can be replicated to a storage account that is owned by the customer. By setting allowCrossTenantReplication to false, objects replication can be configured only if both source and destination accounts are in the same Azure AD tenant. |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountAllowCrossTenantReplication_Audit.json) |
|[Storage accounts should prevent shared key access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F8c6a50c6-9ffd-4ae7-986f-5fa6111f9a54) |Audit requirement of Azure Active Directory (Azure AD) to authorize requests for your storage account. By default, requests can be authorized with either Azure Active Directory credentials, or by using the account access key for Shared Key authorization. Of these two types of authorization, Azure AD provides superior security and ease of use over Shared Key, and is recommended by Microsoft. |Audit, Deny, Disabled |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountAllowSharedKeyAccess_Audit.json) |
|[Storage accounts should restrict network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F34c877ad-507e-4c82-993e-3452a6e0ad3c) |Network access to storage accounts should be restricted. Configure network rules so only applications from allowed networks can access the storage account. To allow connections from specific internet or on-premises clients, access can be granted to traffic from specific Azure virtual networks or to public internet IP address ranges |Audit, Deny, Disabled |[1.1.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/Storage_NetworkAcls_Audit.json) |
|[Storage accounts should restrict network access using virtual network rules](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F2a1a9cdf-e04d-429a-8416-3bfb72a1b26f) |Protect your storage accounts from potential threats using virtual network rules as a preferred method instead of IP-based filtering. Disabling IP-based filtering prevents public IPs from accessing your storage accounts. |Audit, Deny, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountOnlyVnetRulesEnabled_Audit.json) |
|[Storage Accounts should use a virtual network service endpoint](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F60d21c4f-21a3-4d94-85f4-b924e6aeeda4) |This policy audits any Storage Account not configured to use a virtual network service endpoint. |Audit, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Network/VirtualNetworkServiceEndpoint_StorageAccount_Audit.json) |
|[Storage accounts should use customer-managed key for encryption](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F6fac406b-40ca-413b-bf8e-0bf964659c25) |Secure your blob and file storage account with greater flexibility using customer-managed keys. When you specify a customer-managed key, that key is used to protect and control access to the key that encrypts your data. Using customer-managed keys provides additional capabilities to control rotation of the key encryption key or cryptographically erase data. |Audit, Disabled |[1.0.3](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountCustomerManagedKeyEnabled_Audit.json) |
|[Storage accounts should use private link](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F6edd7eda-6dd8-40f7-810d-67160c639cd9) |Azure Private Link lets you connect your virtual network to Azure services without a public IP address at the source or destination. The Private Link platform handles the connectivity between the consumer and services over the Azure backbone network. By mapping private endpoints to your storage account, data leakage risks are reduced. Learn more about private links at - [https://aka.ms/azureprivatelinkoverview](https://aka.ms/azureprivatelinkoverview) |AuditIfNotExists, Disabled |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageAccountPrivateEndpointEnabled_Audit.json) |
|[Table Storage should use customer-managed key for encryption](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F7c322315-e26d-4174-a99e-f49d351b4688) |Secure your table storage with greater flexibility using customer-managed keys. When you specify a customer-managed key, that key is used to protect and control access to the key that encrypts your data. Using customer-managed keys provides additional capabilities to control rotation of the key encryption key or cryptographically erase data. |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Storage/StorageTableCustomerManagedKeyEnabled_Audit.json) |