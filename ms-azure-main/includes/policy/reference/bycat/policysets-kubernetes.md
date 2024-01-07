---
author: davidsmatlak
ms.service: azure-policy
ms.topic: include
ms.date: 01/02/2024
ms.author: davidsmatlak
ms.custom: generated
---

|Name |Description |Policies |Version |
|---|---|---|---|
|[\[Preview\]: Use Image Integrity to ensure only trusted images are deployed](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policySetDefinitions/Kubernetes/AKS_ImageIntegrity.json) |Use Image Integrity to ensure AKS clusters deploy only trusted images by enabling the Image Integrity and Azure Policy Add-Ons on AKS clusters. Image Integrity Add-On and Azure Policy Add-On are both pre-requisites to using Image Integrity to verify if image is signed upon deployment. For more info, visit [https://aka.ms/aks/image-integrity](https://aka.ms/aks/image-integrity). |3 |1.1.0-preview |
|[\[Preview\]: AKS Safeguards should help guide developers towards AKS recommended best practices](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policySetDefinitions/Kubernetes/AKS_Safeguards.json) |A collection of Kubernetes best practices that are recommended by Azure Kubernetes Service (AKS). For the best experience, use AKS Deployment Safeguards to assign this policy initiative: [https://aka.ms/aks/safeguards](https://aka.ms/aks/safeguards). Azure Policy Add-On for AKS is a pre-requisite for applying these best practices to your clusters. For instructions on enabling the Azure Policy Add-On, go to aka.ms/akspolicydoc |11 |1.3.2-preview |
|[Kubernetes cluster pod security baseline standards for Linux-based workloads](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policySetDefinitions/Kubernetes/Kubernetes_PSPBaselineStandard.json) |This initiative includes the policies for the Kubernetes cluster pod security baseline standards. This policy is generally available for Kubernetes Service (AKS), and preview for Azure Arc enabled Kubernetes. For instructions on using this policy, visit [https://aka.ms/kubepolicydoc](https://aka.ms/kubepolicydoc). |5 |1.4.0 |
|[Kubernetes cluster pod security restricted standards for Linux-based workloads](https://github.com/Azure/azure-policy/blob/master/built-in-policies/policySetDefinitions/Kubernetes/Kubernetes_PSPRestrictedStandard.json) |This initiative includes the policies for the Kubernetes cluster pod security restricted standards. This policy is generally available for Kubernetes Service (AKS), and preview for Azure Arc enabled Kubernetes. For instructions on using this policy, visit [https://aka.ms/kubepolicydoc](https://aka.ms/kubepolicydoc). |8 |2.4.0 |