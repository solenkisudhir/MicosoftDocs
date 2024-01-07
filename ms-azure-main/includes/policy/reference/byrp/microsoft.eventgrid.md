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
|[Azure Event Grid domains should disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ff8f774be-6aee-492a-9e29-486ef81f3a68) |Disabling public network access improves security by ensuring that the resource isn't exposed on the public internet. You can limit exposure of your resources by creating private endpoints instead. Learn more at: [https://aka.ms/privateendpoints](https://aka.ms/privateendpoints). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Domains_PublicNetworkAccess_AuditDeny.json) |
|[Azure Event Grid domains should have local authentication methods disabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F8bfadddb-ee1c-4639-8911-a38cb8e0b3bd) |Disabling local authentication methods improves security by ensuring that Azure Event Grid domains exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/aeg-disablelocalauth](https://aka.ms/aeg-disablelocalauth). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Domains_DisableLocalAuth_AuditDeny.json) |
|[Azure Event Grid domains should use private link](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F9830b652-8523-49cc-b1b3-e17dce1127ca) |Azure Private Link lets you connect your virtual network to Azure services without a public IP address at the source or destination. The Private Link platform handles the connectivity between the consumer and services over the Azure backbone network. By mapping private endpoints to your Event Grid domain instead of the entire service, you'll also be protected against data leakage risks. Learn more at: [https://aka.ms/privateendpoints](https://aka.ms/privateendpoints). |Audit, Disabled |[1.0.2](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Domains_PrivateEndpoint_Audit.json) |
|[Azure Event Grid namespace MQTT broker should use private link](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fcd8f7644-6fe8-4516-bded-0e465ead03ac) |Azure Private Link lets you connect your virtual network to Azure services without a public IP address at the source or destination. The Private Link platform handles the connectivity between the consumer and services over the Azure backbone network. By mapping private endpoints to your Event Grid namespace instead of the entire service, you'll also be protected against data leakage risks. Learn more at: [https://aka.ms/aeg-ns-privateendpoints](https://aka.ms/aeg-ns-privateendpoints). |Audit, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/NamespaceMQTTBroker_PrivateEndpoint_Audit.json) |
|[Azure Event Grid namespace topic broker should use private link](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F1301a000-bc6b-4d90-8414-7091e3abdc40) |Azure Private Link lets you connect your virtual network to Azure services without a public IP address at the source or destination. The Private Link platform handles the connectivity between the consumer and services over the Azure backbone network. By mapping private endpoints to your Event Grid namespace instead of the entire service, you'll also be protected against data leakage risks. Learn more at: [https://aka.ms/aeg-ns-privateendpoints](https://aka.ms/aeg-ns-privateendpoints). |Audit, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/NamespaceTopic_PrivateEndpoint_Audit.json) |
|[Azure Event Grid namespaces should disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F67dcad1a-ec60-45df-8fd0-14c9d29eeaa2) |Disabling public network access improves security by ensuring that the resource isn't exposed on the public internet. You can limit exposure of your resources by creating private endpoints instead. Learn more at: [https://aka.ms/aeg-ns-privateendpoints](https://aka.ms/aeg-ns-privateendpoints). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Namespaces_PublicNetworkAccess_AuditDeny.json) |
|[Azure Event Grid partner namespaces should have local authentication methods disabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F8632b003-3545-4b29-85e6-b2b96773df1e) |Disabling local authentication methods improves security by ensuring that Azure Event Grid partner namespaces exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/aeg-disablelocalauth](https://aka.ms/aeg-disablelocalauth). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/PartnerNamespaces_DisableLocalAuth_AuditDeny.json) |
|[Azure Event Grid topics should disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F1adadefe-5f21-44f7-b931-a59b54ccdb45) |Disabling public network access improves security by ensuring that the resource isn't exposed on the public internet. You can limit exposure of your resources by creating private endpoints instead. Learn more at: [https://aka.ms/privateendpoints](https://aka.ms/privateendpoints). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Topics_PublicNetworkAccess_AuditDeny.json) |
|[Azure Event Grid topics should have local authentication methods disabled](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fae9fb87f-8a17-4428-94a4-8135d431055c) |Disabling local authentication methods improves security by ensuring that Azure Event Grid topics exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/aeg-disablelocalauth](https://aka.ms/aeg-disablelocalauth). |Audit, Deny, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Topics_DisableLocalAuth_AuditDeny.json) |
|[Azure Event Grid topics should use private link](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F4b90e17e-8448-49db-875e-bd83fb6f804f) |Azure Private Link lets you connect your virtual network to Azure services without a public IP address at the source or destination. The Private Link platform handles the connectivity between the consumer and services over the Azure backbone network. By mapping private endpoints to your Event Grid topic instead of the entire service, you'll also be protected against data leakage risks. Learn more at: [https://aka.ms/privateendpoints](https://aka.ms/privateendpoints). |Audit, Disabled |[1.0.2](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Topics_PrivateEndpoint_Audit.json) |
|[Configure Azure Event Grid domains to disable local authentication](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F8ac2748f-3bf1-4c02-a3b6-92ae68cf75b1) |Disable local authentication methods so that your Azure Event Grid domains exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/aeg-disablelocalauth](https://aka.ms/aeg-disablelocalauth). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Domains_DisableLocalAuth_Modify.json) |
|[Configure Azure Event Grid namespace MQTT broker with private endpoints](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fcddcbb7e-a7b1-4380-b4d8-45cf77b0d561) |Private endpoints lets you connect your virtual network to Azure services without a public IP address at the source or destination. By mapping private endpoints to your resources, they'll be protected against data leakage risks. Learn more at: [https://aka.ms/aeg-ns-privateendpoints](https://aka.ms/aeg-ns-privateendpoints). |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/NamespaceMQTTBroker_PrivateEndpoint_DeployIfNotExists.json) |
|[Configure Azure Event Grid namespaces with private endpoints](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F2b21ce34-9c45-4037-9c84-0ac0dbd0095f) |Private endpoints lets you connect your virtual network to Azure services without a public IP address at the source or destination. By mapping private endpoints to your resources, they'll be protected against data leakage risks. Learn more at: [https://aka.ms/aeg-ns-privateendpoints](https://aka.ms/aeg-ns-privateendpoints). |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/NamespaceTopic_PrivateEndpoint_DeployIfNotExists.json) |
|[Configure Azure Event Grid partner namespaces to disable local authentication](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F2dd0e8b9-4289-4bb0-b813-1883298e9924) |Disable local authentication methods so that your Azure Event Grid partner namespaces exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/aeg-disablelocalauth](https://aka.ms/aeg-disablelocalauth). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/PartnerNamespaces_DisableLocalAuth_Modify.json) |
|[Configure Azure Event Grid topics to disable local authentication](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F1c8144d9-746a-4501-b08c-093c8d29ad04) |Disable local authentication methods so that your Azure Event Grid topics exclusively require Azure Active Directory identities for authentication. Learn more at: [https://aka.ms/aeg-disablelocalauth](https://aka.ms/aeg-disablelocalauth). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Topics_DisableLocalAuth_Modify.json) |
|[Deploy - Configure Azure Event Grid domains with private endpoints](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F36f4658a-848a-467b-881c-e6fa20cf75fc) |Private endpoints lets you connect your virtual network to Azure services without a public IP address at the source or destination. By mapping private endpoints to your resources, they'll be protected against data leakage risks. Learn more at: [https://aka.ms/privateendpoints](https://aka.ms/privateendpoints). |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Domains_PrivateEndpoint_DeployIfNotExists.json) |
|[Deploy - Configure Azure Event Grid topics with private endpoints](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F6fcec95c-fbdf-45e8-91e1-e3175d9c9eca) |Private endpoints lets you connect your virtual network to Azure services without a public IP address at the source or destination. By mapping private endpoints to your resources, they'll be protected against data leakage risks. Learn more at: [https://aka.ms/privateendpoints](https://aka.ms/privateendpoints). |DeployIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Topics_PrivateEndpoint_DeployIfNotExists.json) |
|[Enable logging by category group for Event Grid Domains (microsoft.eventgrid/domains) to Event Hub](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fa81eb966-6696-46b1-9153-bed01569a7d0) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to an Event Hub for Event Grid Domains (microsoft.eventgrid/domains). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_eventHub_eventgrid-domains_DINE.json) |
|[Enable logging by category group for Event Grid Domains (microsoft.eventgrid/domains) to Log Analytics](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fb90ec596-faa6-4c61-9515-34085703e260) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to a Log Analytics workspace for Event Grid Domains (microsoft.eventgrid/domains). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_logAnalytics_eventgrid-domains_DINE.json) |
|[Enable logging by category group for Event Grid Domains (microsoft.eventgrid/domains) to Storage](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F03a087c0-b49f-4440-9ae5-013703eccc8c) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to a Storage Account for Event Grid Domains (microsoft.eventgrid/domains). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/AzureMonitor_DiagSettings_storage_eventgrid-domains_Deploy.json) |
|[Enable logging by category group for Event Grid Partner Namespaces (microsoft.eventgrid/partnernamespaces) to Event Hub](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ff6d5d5d5-0fa9-4257-b820-69c35016c973) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to an Event Hub for Event Grid Partner Namespaces (microsoft.eventgrid/partnernamespaces). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_eventHub_eventgrid-partnernamespaces_DINE.json) |
|[Enable logging by category group for Event Grid Partner Namespaces (microsoft.eventgrid/partnernamespaces) to Log Analytics](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F3496f6fd-57ba-485c-8a14-183c4493b781) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to a Log Analytics workspace for Event Grid Partner Namespaces (microsoft.eventgrid/partnernamespaces). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_logAnalytics_eventgrid-partnernamespaces_DINE.json) |
|[Enable logging by category group for Event Grid Partner Namespaces (microsoft.eventgrid/partnernamespaces) to Storage](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ff873a711-0322-4744-8322-7e62950fbec2) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to a Storage Account for Event Grid Partner Namespaces (microsoft.eventgrid/partnernamespaces). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_storage_eventgrid-partnernamespaces_DINE.json) |
|[Enable logging by category group for Event Grid Topics (microsoft.eventgrid/topics) to Event Hub](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ff5094957-e0f7-4af2-9e14-13d60141dc4a) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to an Event Hub for Event Grid Topics (microsoft.eventgrid/topics). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_eventHub_eventgrid-topics_DINE.json) |
|[Enable logging by category group for Event Grid Topics (microsoft.eventgrid/topics) to Log Analytics](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F46b2dd5d-3936-4347-8908-b298ea4466d3) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to a Log Analytics workspace for Event Grid Topics (microsoft.eventgrid/topics). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/DiagSettings_logAnalytics_eventgrid-topics_DINE.json) |
|[Enable logging by category group for Event Grid Topics (microsoft.eventgrid/topics) to Storage](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ffcfe6bfa-dd36-40ef-ab2b-ed46f7d4abdb) |Resource logs should be enabled to track activities and events that take place on your resources and give you visibility and insights into any changes that occur. This policy deploys a diagnostic setting using a category group to route logs to a Storage Account for Event Grid Topics (microsoft.eventgrid/topics). |DeployIfNotExists, AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Monitoring/AzureMonitor_DiagSettings_storage_eventgrid-topics_Deploy.json) |
|[Modify - Configure Azure Event Grid domains to disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F898e9824-104c-4965-8e0e-5197588fa5d4) |Disable public network access for Azure Event Grid resource so that it isn't accessible over the public internet. This will help protect them against data leakage risks. You can limit exposure of the your resources by creating private endpoints instead. Learn more at: [https://aka.ms/privateendpoints](https://aka.ms/privateendpoints). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Domains_PublicNetworkAccess_Modify.json) |
|[Modify - Configure Azure Event Grid topics to disable public network access](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F36ea4b4b-0f7f-4a54-89fa-ab18f555a172) |Disable public network access for Azure Event Grid resource so that it isn't accessible over the public internet. This will help protect them against data leakage risks. You can limit exposure of the your resources by creating private endpoints instead. Learn more at: [https://aka.ms/privateendpoints](https://aka.ms/privateendpoints). |Modify, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Event%20Grid/Topics_PublicNetworkAccess_Modify.json) |