
# Azure Blueprint Extension for Azure Pipelines (product strategy)

## Vision

To provide Azure Blueprint creation and management capabilities, from an Azure Pipeline, without requiring custom code.

### Objectives

Provide the necessary tooling for managing Azure Blueprints from within an Azure Pipeline. Using the Azure Blueprint extensions for Azure Pipelines, customers can store pipeline definitions in source control, create Azure blueprints from this source, and assign these blueprints using Azure blueprint specific pipeline tasks. These pipeline tasks function without the requirement of custom code.

### Customer

Cloud operators who are engaged in infrastructure and governance operations using continuous deployment with Azure Pipelines.

### Need

The use of continuous deployment solutions is expanding to include infrastructure, policy, and other operations related tasks. 

Currently, Azure Blueprints have two interfaces, the Azure Portal and a PowerShell module. For customers to manage Azure Blueprints from an Azure Pipeline, code needs to be written and embedded using the Azure Blueprint PowerShell module and a generic Azure Pipeline task such as the task for PowerShell. This method requires comfort writing PowerShell scripts.

Providing a native Azure Pipeline activity for preforming Blueprint deployments enables anyone, regardless of scripting knowledge to build and use deployment pipelines that include Azure Blueprints.

### Competiton and Differentiation

Several governance-related extensions have been created for Azure Pipeline. Most of these are sourced from hobbyists and community members.

## Goals

| Goal | Metric |
|---|---|
| Provide Blueprint create and assignment functionality from Azure Pipelines. | Can I create and assign an Azure Blueprint with the task? |
| Provide accurate and complete documentation for the extension. | Complete documentation coverage for each feature and configuration. Documentation needs to address both UI and YAML configurations. |
| Provide timely support response and resolution. | Respond to GitHub issues and pull requests within 7 days. Close issues and pull requests within 3 weeks. |
| Ensure steady usage growth | 200 installations within the first 6 months, and then 1 daily thereafter. |

## Initiatives

