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
|[\[Preview\]: System updates should be installed on your machines (powered by Update Center)](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ff85bf3e0-d513-442e-89c3-1784ad63382b) |Your machines are missing system, security, and critical updates. Software updates often include critical patches to security holes. Such holes are frequently exploited in malware attacks so it's vital to keep your software updated. To install all outstanding patches and secure your machines, follow the remediation steps. |AuditIfNotExists, Disabled |[1.0.0-preview](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/ASC_MissingSystemUpdatesV2_Audit.json) |
|[Container registry images should have vulnerability findings resolved](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F5f0f936f-2f01-4bf5-b6be-d423792fa562) |Container image vulnerability assessment scans your registry for security vulnerabilities and exposes detailed findings for each image. Resolving the vulnerabilities can greatly improve your containers' security posture and protect them from attacks. |AuditIfNotExists, Disabled |[2.0.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/ASC_ContainerRegistryVulnerabilityAssessment_Audit.json) |
|[Container registry images should have vulnerability findings resolved (powered by Microsoft Defender Vulnerability Management)](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F090c7b07-b4ed-4561-ad20-e9075f3ccaff) |Container image vulnerability assessment scans your registry for commonly known vulnerabilities (CVEs) and provides a detailed vulnerability report for each image. Resolving vulnerabilities can greatly improve your security posture, ensuring images are safe to use prior to deployment. |AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/MDC_AzureContainerRegistryVulnerabilityAssessment_Audit.json) |
|[Machines should be configured to periodically check for missing system updates](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fbd876905-5b84-4f73-ab2d-2e7a7c4568d9) |To ensure periodic assessments for missing system updates are triggered automatically every 24 hours, the AssessmentMode property should be set to 'AutomaticByPlatform'. Learn more about AssessmentMode property for Windows: [https://aka.ms/computevm-windowspatchassessmentmode,](https://aka.ms/computevm-windowspatchassessmentmode,) for Linux: [https://aka.ms/computevm-linuxpatchassessmentmode](https://aka.ms/computevm-linuxpatchassessmentmode). |Audit, Deny, Disabled |[3.4.1](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Azure%20Update%20Manager/AzUpdateMgmtCenter_AutoAssessmentMode_Audit.json) |
|[Running container images should have vulnerability findings resolved](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F0fc39691-5a3f-4e3e-94ee-2e6447309ad9) |Container image vulnerability assessment scans container images running on your Kubernetes clusters for security vulnerabilities and exposes detailed findings for each image. Resolving the vulnerabilities can greatly improve your containers' security posture and protect them from attacks. |AuditIfNotExists, Disabled |[1.0.2](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/ASC_KuberenetesRuningImagesVulnerabilityAssessment_Audit.json) |
|[Running container images should have vulnerability findings resolved (powered by Microsoft Defender Vulnerability Management)](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F17f4b1cc-c55c-4d94-b1f9-2978f6ac2957) |Container image vulnerability assessment scans your registry for commonly known vulnerabilities (CVEs) and provides a detailed vulnerability report for each image. This recommendation provides visibility to vulnerable images currently running in your Kubernetes clusters. Remediating vulnerabilities in container images that are currently running is key to improving your security posture, significantly reducing the attack surface for your containerized workloads. |AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/MDC_K8sRuningImagesVulnerabilityAssessmentBasedOnMDVM_Audit.json) |
|[SQL databases should have vulnerability findings resolved](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Ffeedbf84-6b99-488c-acc2-71c829aa5ffc) |Monitor vulnerability assessment scan results and recommendations for how to remediate database vulnerabilities. |AuditIfNotExists, Disabled |[4.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/ASC_SQLDbVulnerabilities_Audit.json) |
|[SQL servers on machines should have vulnerability findings resolved](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F6ba6d016-e7c3-4842-b8f2-4992ebc0d72d) |SQL vulnerability assessment scans your database for security vulnerabilities, and exposes any deviations from best practices such as misconfigurations, excessive permissions, and unprotected sensitive data. Resolving the vulnerabilities found can greatly improve your database security posture. |AuditIfNotExists, Disabled |[1.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/ASC_ServerSQLVulnerabilityAssessment_Audit.json) |
|[System updates on virtual machine scale sets should be installed](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fc3f317a7-a95c-4547-b7e7-11017ebdf2fe) |Audit whether there are any missing system security updates and critical updates that should be installed to ensure that your Windows and Linux virtual machine scale sets are secure. |AuditIfNotExists, Disabled |[3.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/ASC_VmssMissingSystemUpdates_Audit.json) |
|[System updates should be installed on your machines](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F86b3d65f-7626-441e-b690-81a8b71cff60) |Missing security system updates on your servers will be monitored by Azure Security Center as recommendations |AuditIfNotExists, Disabled |[4.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/ASC_MissingSystemUpdates_Audit.json) |
|[Vulnerabilities in container security configurations should be remediated](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fe8cbc669-f12d-49eb-93e7-9273119e9933) |Audit vulnerabilities in security configuration on machines with Docker installed and display as recommendations in Azure Security Center. |AuditIfNotExists, Disabled |[3.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/ASC_ContainerBenchmark_Audit.json) |
|[Vulnerabilities in security configuration on your machines should be remediated](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2Fe1e5fd5d-3e4c-4ce1-8661-7d1873ae6b15) |Servers which do not satisfy the configured baseline will be monitored by Azure Security Center as recommendations |AuditIfNotExists, Disabled |[3.1.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/ASC_OSVulnerabilities_Audit.json) |
|[Vulnerabilities in security configuration on your virtual machine scale sets should be remediated](https://portal.azure.com/#blade/Microsoft_Azure_Policy/PolicyDetailBlade/definitionId/%2Fproviders%2FMicrosoft.Authorization%2FpolicyDefinitions%2F3c735d8a-a4ba-4a3a-b7cf-db7754cf57f4) |Audit the OS vulnerabilities on your virtual machine scale sets to protect them from attacks. |AuditIfNotExists, Disabled |[3.0.0](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policyDefinitions/Security%20Center/ASC_VmssOSVulnerabilities_Audit.json) |