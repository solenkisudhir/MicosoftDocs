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
|[\[Preview\]: SQL Databases should be Zone Redundant](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F6221cac0-bb8d-40f4-9535-5d03f713f054) |SQL Databases can be configured to be Zone Redundant or not. Databases with the 'zoneRedundant' setting set to 'false' are not configured for zone redundancy. This policy helps identify SQL databases that need zone redundancy configuration to enhance availability and resilience within Azure. |Audit, Deny, Disabled |[1.0.0-preview](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Resilience/Sql_servers_databases_ZoneRedundant_Audit.json) |
|[\[Preview\]: SQL Elastic database pools should be Zone Redundant](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ff16a3ca9-b57a-4392-b660-4c1f8442aa8d) |SQL Elastic database pools can be configured to be Zone Redundant or not. SQL Elastic database pools are Zone Redundant if it's 'zoneRedundant' property is set to 'true'. Enforcing this policy helps ensure that Event Hubs are appropriately configured for zone resilience, reducing the risk of downtime during zone outages. |Audit, Deny, Disabled |[1.0.0-preview](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Resilience/Sql_servers_elasticpools_ZoneRedundant_Audit.json) |
|[\[Preview\]: SQL Managed Instances should be Zone Redundant](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F0fc92280-604b-4f23-9e04-5ef98d1a28df) |SQL Managed Instances can be configured to be Zone Redundant or not. Instances with the 'zoneRedundant' setting set to 'false' are not configured for zone redundancy. This policy helps identify SQL managedInstances that need zone redundancy configuration to enhance availability and resilience within Azure. |Audit, Deny, Disabled |[1.0.0-preview](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Resilience/Sql_managedInstances_ZoneRedundant_Audit.json) |
|[An Azure Active Directory administrator should be provisioned for SQL servers](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F1f314764-cb73-4fc9-b863-8eca98ac36e9) |Audit provisioning of an Azure Active Directory administrator for your SQL server to enable Azure AD authentication. Azure AD authentication enables simplified permission management and centralized identity management of database users and other Microsoft services |AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SQL_DB_AuditServerADAdmins_Audit.json) |
|[Auditing on SQL server should be enabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fa6fb4358-5bf4-4ad7-ba82-2cd2f41ce5e9) |Auditing on your SQL Server should be enabled to track database activities across all databases on the server and save them in an audit log. |AuditIfNotExists, Disabled |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServerAuditing_Audit.json) |
|[Azure Defender for SQL should be enabled for unprotected Azure SQL servers](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fabfb4388-5bf4-4ad7-ba82-2cd2f41ceae9) |Audit SQL servers without Advanced Data Security |AuditIfNotExists, Disabled |[2.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServer_AdvancedDataSecurity_Audit.json) |
|[Azure Defender for SQL should be enabled for unprotected SQL Managed Instances](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fabfb7388-5bf4-4ad7-ba99-2cd2f41cebb9) |Audit each SQL Managed Instance without advanced data security. |AuditIfNotExists, Disabled |[1.0.2](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlManagedInstance_AdvancedDataSecurity_Audit.json) |
|[Azure SQL Database should be running TLS version 1.2 or newer](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F32e6bbec-16b6-44c2-be37-c5b672d103cf) |Setting TLS version to 1.2 or newer improves security by ensuring your Azure SQL Database can only be accessed from clients using TLS 1.2 or newer. Using versions of TLS less than 1.2 is not recommended since they have well documented security vulnerabilities. |Audit, Disabled, Deny |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServer_MiniumTLSVersion_Audit.json) |
|[Azure SQL Database should have Microsoft Entra-only authentication enabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fabda6d70-9778-44e7-84a8-06713e6db027) |Disabling local authentication methods and allowing only Microsoft Entra authentication improves security by ensuring that Azure SQL Databases can exclusively be accessed by Microsoft Entra identities. Learn more at: aka.ms/adonlycreate. |Audit, Deny, Disabled |[1.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServer_ADOnlyEnabled_Deny.json) |
|[Azure SQL Managed Instance should have Microsoft Entra-only authentication enabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F78215662-041e-49ed-a9dd-5385911b3a1f) |Disabling local authentication methods and allowing only Microsoft Entra authentication improves security by ensuring that Azure SQL Managed Instances can exclusively be accessed by Microsoft Entra identities. Learn more at: aka.ms/adonlycreate. |Audit, Deny, Disabled |[1.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlManagedInstance_ADOnlyEnabled_Deny.json) |
|[Azure SQL Managed Instances should disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F9dfea752-dd46-4766-aed1-c355fa93fb91) |Disabling public network access (public endpoint) on Azure SQL Managed Instances improves security by ensuring that they can only be accessed from inside their virtual networks or via Private Endpoints. To learn more about public network access, visit [https://aka.ms/mi-public-endpoint](https://aka.ms/mi-public-endpoint). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlManagedInstance_PublicEndpoint_Audit.json) |
|[Configure Azure Defender to be enabled on SQL managed instances](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fc5a62eb0-c65a-4220-8a4d-f70dd4ca95dd) |Enable Azure Defender on your Azure SQL Managed Instances to detect anomalous activities indicating unusual and potentially harmful attempts to access or exploit databases. |DeployIfNotExists, Disabled |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/TdOnManagedInstances_Deploy.json) |
|[Configure Azure Defender to be enabled on SQL servers](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F36d49e87-48c4-4f2e-beed-ba4ed02b71f5) |Enable Azure Defender on your Azure SQL Servers to detect anomalous activities indicating unusual and potentially harmful attempts to access or exploit databases. |DeployIfNotExists |[2.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/TdOnSqlServers_Deploy.json) |
|[Configure Azure SQL database servers diagnostic settings to Log Analytics workspace](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F7ea8a143-05e3-4553-abfe-f56bef8b0b70) |Enables auditing logs for Azure SQL Database server and stream the logs to a Log Analytics workspace when any SQL Server which is missing this auditing is created or updated |DeployIfNotExists, Disabled |[1.0.2](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/DataConnectosSqServerLogs_PolicyAssignment.json) |
|[Configure Azure SQL Server to disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F28b0b1e5-17ba-4963-a7a4-5a1ab4400a0b) |Disabling the public network access property shuts down public connectivity such that Azure SQL Server can only be accessed from a private endpoint. This configuration disables the public network access for all databases under the Azure SQL Server. |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServer_PublicNetworkAccess_Modify.json) |
|[Configure Azure SQL Server to enable private endpoint connections](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F8e8ca470-d980-4831-99e6-dc70d9f6af87) |A private endpoint connection enables private connectivity to your Azure SQL Database via a private IP address inside a virtual network. This configuration improves your security posture and supports Azure networking tools and scenarios. |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServer_PrivateEndpoint_DeployIfNotExists.json) |
|[Configure SQL servers to have auditing enabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ff4c68484-132f-41f9-9b6d-3e4b1cb55036) |To ensure the operations performed against your SQL assets are captured, SQL servers should have auditing enabled. This is sometimes required for compliance with regulatory standards. |DeployIfNotExists, Disabled |[3.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServerAuditing_Deploy.json) |
|[Configure SQL servers to have auditing enabled to Log Analytics workspace](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F25da7dfb-0666-4a15-a8f5-402127efd8bb) |To ensure the operations performed against your SQL assets are captured, SQL servers should have auditing enabled. If auditing is not enabled, this policy will configure auditing events to flow to the specified Log Analytics workspace. |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServerAuditingToLA_Deploy.json) |
|[Deploy - Configure diagnostic settings for SQL Databases to Log Analytics workspace](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fb79fa14e-238a-4c2d-b376-442ce508fc84) |Deploys the diagnostic settings for SQL Databases to stream resource logs to a Log Analytics workspace when any SQL Database which is missing this diagnostic settings is created or updated. |DeployIfNotExists, Disabled |[4.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/DataConnectosSqlLogs_PolicyAssignment.json) |
|[Deploy Advanced Data Security on SQL servers](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F6134c3db-786f-471e-87bc-8f479dc890f6) |This policy enables Advanced Data Security on SQL Servers. This includes turning on Threat Detection and Vulnerability Assessment. It will automatically create a storage account in the same region and resource group as the SQL server to store scan results, with a 'sqlva' prefix. |DeployIfNotExists |[1.3.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServerAdvancedDataSecurity_Deploy.json) |
|[Deploy Diagnostic Settings for Azure SQL Database to Event Hub](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F9a7c7a7d-49e5-4213-bea8-6a502b6272e0) |Deploys the diagnostic settings for Azure SQL Database to stream to a regional Event Hub on any Azure SQL Database which is missing this diagnostic settings is created or updated. |DeployIfNotExists |[1.2.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlDB_DiagnosticsLog_Deploy.json) |
|[Deploy SQL DB transparent data encryption](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F86a912f6-9a06-4e26-b447-11b16ba8659f) |Enables transparent data encryption on SQL databases |DeployIfNotExists, Disabled |[2.2.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlDBEncryption_Deploy.json) |
|[Enable logging by category group for SQL databases (microsoft.sql/servers/databases) to Event Hub](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F9e6aee71-3781-4acd-bba7-aac4fb067dfa) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to an Event Hub for SQL databases (microsoft.sql/servers/databases). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_eventHub_sql-servers-databases_DINE.json) |
|[Enable logging by category group for SQL databases (microsoft.sql/servers/databases) to Log Analytics](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F6567d3f3-42d0-4cfb-9606-9741ba60fa07) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to a Log Analytics workspace for SQL databases (microsoft.sql/servers/databases). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_logAnalytics_sql-servers-databases_DINE.json) |
|[Enable logging by category group for SQL databases (microsoft.sql/servers/databases) to Storage](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F8656d368-0643-4374-a63f-ae0ed4da1d9a) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to a Storage Account for SQL databases (microsoft.sql/servers/databases). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_storage_sql-servers-databases_DINE.json) |
|[Enable logging by category group for SQL managed instances (microsoft.sql/managedinstances) to Event Hub](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F5f6f2aba-e57f-42ed-9aeb-ffa7321a56db) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to an Event Hub for SQL managed instances (microsoft.sql/managedinstances). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_eventHub_sql-managedinstances_DINE.json) |
|[Enable logging by category group for SQL managed instances (microsoft.sql/managedinstances) to Log Analytics](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F8fc4ca5f-6abc-4b30-9565-0bd91ac49420) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to a Log Analytics workspace for SQL managed instances (microsoft.sql/managedinstances). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_logAnalytics_sql-managedinstances_DINE.json) |
|[Enable logging by category group for SQL managed instances (microsoft.sql/managedinstances) to Storage](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F40654dcd-0b26-49d6-aeaf-d12d7c1e8c4d) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to a Storage Account for SQL managed instances (microsoft.sql/managedinstances). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_storage_sql-managedinstances_DINE.json) |
|[Long-term geo-redundant backup should be enabled for Azure SQL Databases](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fd38fc420-0735-4ef3-ac11-c806f651a570) |This policy audits any Azure SQL Database with long-term geo-redundant backup not enabled. |AuditIfNotExists, Disabled |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/GeoRedundant_SQLDatabase_AuditIfNotExists.json) |
|[Private endpoint connections on Azure SQL Database should be enabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F7698e800-9299-47a6-b3b6-5a0fee576eed) |Private endpoint connections enforce secure communication by enabling private connectivity to Azure SQL Database. |Audit, Disabled |[1.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServer_PrivateEndpoint_Audit.json) |
|[Public network access on Azure SQL Database should be disabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F1b8ca024-1d5c-4dec-8995-b1a932b41780) |Disabling the public network access property improves security by ensuring your Azure SQL Database can only be accessed from a private endpoint. This configuration denies all logins that match IP or virtual network based firewall rules. |Audit, Deny, Disabled |[1.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServer_PublicNetworkAccess_Audit.json) |
|[SQL Auditing settings should have Action-Groups configured to capture critical activities](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F7ff426e2-515f-405a-91c8-4f2333442eb5) |The AuditActionsAndGroups property should contain at least SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP, BATCH_COMPLETED_GROUP to ensure a thorough audit logging |AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServerAuditing_ActionsAndGroups_Audit.json) |
|[SQL Database should avoid using GRS backup redundancy](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fb219b9cf-f672-4f96-9ab0-f5a3ac5e1c13) |Databases should avoid using the default geo-redundant storage for backups, if data residency rules require data to stay within a specific region. Note: Azure Policy is not enforced when creating a database using T-SQL. If not explicitly specified, database with geo-redundant backup storage is created via T-SQL. |Deny, Disabled |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlDb_BlockGrsBackupRedundancy_Deny.json) |
|[SQL databases should have vulnerability findings resolved](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ffeedbf84-6b99-488c-acc2-71c829aa5ffc) |Monitor vulnerability assessment scan results and recommendations for how to remediate database vulnerabilities. |AuditIfNotExists, Disabled |[4.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/ASC_SQLDbVulnerabilities_Audit.json) |
|[SQL Managed Instance should have the minimal TLS version of 1.2](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fa8793640-60f7-487c-b5c3-1d37215905c4) |Setting minimal TLS version to 1.2 improves security by ensuring your SQL Managed Instance can only be accessed from clients using TLS 1.2. Using versions of TLS less than 1.2 is not recommended since they have well documented security vulnerabilities. |Audit, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlManagedInstance_MiniumTLSVersion_Audit.json) |
|[SQL Managed Instances should avoid using GRS backup redundancy](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fa9934fd7-29f2-4e6d-ab3d-607ea38e9079) |Managed Instances should avoid using the default geo-redundant storage for backups, if data residency rules require data to stay within a specific region. Note: Azure Policy is not enforced when creating a database using T-SQL. If not explicitly specified, database with geo-redundant backup storage is created via T-SQL. |Deny, Disabled |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlManagedInstance_BlockGrsBackupRedundancy_Deny.json) |
|[SQL managed instances should use customer-managed keys to encrypt data at rest](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fac01ad65-10e5-46df-bdd9-6b0cad13e1d2) |Implementing Transparent Data Encryption (TDE) with your own key provides you with increased transparency and control over the TDE Protector, increased security with an HSM-backed external service, and promotion of separation of duties. This recommendation applies to organizations with a related compliance requirement. |Audit, Deny, Disabled |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlManagedInstance_EnsureServerTDEisEncrypted_Deny.json) |
|[SQL Server should use a virtual network service endpoint](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fae5d2f14-d830-42b6-9899-df6cfe9c71a3) |This policy audits any SQL Server not configured to use a virtual network service endpoint. |AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Network/VirtualNetworkServiceEndpoint_SQLServer_AuditIfNotExists.json) |
|[SQL servers should use customer-managed keys to encrypt data at rest](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F0a370ff3-6cab-4e85-8995-295fd854c5b8) |Implementing Transparent Data Encryption (TDE) with your own key provides increased transparency and control over the TDE Protector, increased security with an HSM-backed external service, and promotion of separation of duties. This recommendation applies to organizations with a related compliance requirement. |Audit, Deny, Disabled |[2.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServer_EnsureServerTDEisEncryptedWithYourOwnKey_Deny.json) |
|[SQL servers with auditing to storage account destination should be configured with 90 days retention or higher](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F89099bee-89e0-4b26-a5f4-165451757743) |For incident investigation purposes, we recommend setting the data retention for your SQL Server' auditing to storage account destination to at least 90 days. Confirm that you are meeting the necessary retention rules for the regions in which you are operating. This is sometimes required for compliance with regulatory standards. |AuditIfNotExists, Disabled |[3.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServerAuditingRetentionDays_Audit.json) |
|[Transparent Data Encryption on SQL databases should be enabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F17k78e20-9358-41c9-923c-fb736d382a12) |Transparent data encryption should be enabled to protect data-at-rest and meet compliance requirements |AuditIfNotExists, Disabled |[2.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlDBEncryption_Audit.json) |
|[Virtual network firewall rule on Azure SQL Database should be enabled to allow traffic from the specified subnet](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F77e8b146-0078-4fb2-b002-e112381199f0) |Virtual network based firewall rules are used to enable traffic from a specific subnet to Azure SQL Database while ensuring the traffic stays within the Azure boundary. |AuditIfNotExists |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/SqlServer_VNetRules_Audit.json) |
|[Vulnerability assessment should be enabled on SQL Managed Instance](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F1b7aa243-30e4-4c9e-bca8-d0d3022b634a) |Audit each SQL Managed Instance which doesn't have recurring vulnerability assessment scans enabled. Vulnerability assessment can discover, track, and help you remediate potential database vulnerabilities. |AuditIfNotExists, Disabled |[1.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/VulnerabilityAssessmentOnManagedInstance_Audit.json) |
|[Vulnerability assessment should be enabled on your SQL servers](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fef2a8f2a-b3d9-49cd-a8a8-9a3aaaf647d9) |Audit Azure SQL servers which do not have vulnerability assessment properly configured. Vulnerability assessment can discover, track, and help you remediate potential database vulnerabilities. |AuditIfNotExists, Disabled |[3.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/SQL/VulnerabilityAssessmentOnServer_Audit.json) |