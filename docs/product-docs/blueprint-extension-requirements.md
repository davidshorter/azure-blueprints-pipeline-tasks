# Azure Pipeline extension for Azure Blueprints requirements

## Product overview and use case

The Azure Pipeline extension for Azure Blueprints will provide native pipeline tasks for creating and assigning Azure Blueprints. With these tasks, consumers can include Blueprint deployments and updates in continuous delivery solutions.

## User stories

### Authentication

| ID | Requirement | Complete |
|:---|---|---|
| 1 | I should be able to authenticate to an Azure Subscription using a Service Principal object. | Yes |
| [52](https://github.com/neilpeterson/azure-blueprints-pipeline-tasks/issues/52) | I should be able to authenticate to an Azure Subscription using a Managed Service Identity object. | No |

### Blueprint Creation Scope

| ID | Requirement | Complete |
|:---|---|---|
| 2 | I should be able to create a Blueprint at the Management Group scope. | Yes |
| 3| I should be able to create a Blueprint at the Subscription scope. | Yes |
| 4 | I should be able to assign a Blueprint stored at an MG scope to a subscription. | Yes |
| 5 | I should be able to assign a Blueprint stored at a subscription scope to the same subscription. | Yes |

### Blueprint Creation

| ID | Requirement | Complete |
|:---|---|---|
| 6 | I should be able to give the blueprint a unique name | Yes |
| 7 | I should be able to provide a directory to the Blueprint definition file | Yes |
| 8 | When using the Azure Pipelines classic editor, I should be able to browse source control for the Blueprint definition. | Yes |
| 9 | When creating a Blueprint, I should be able to publish the Blueprint | Yes |
| 10 | When creating a Blueprint, I should be able to not publish the Blueprint. | Yes |
| 11 | When creating a BLueprint, I should be able to specify a version. | Yes |

### Updating a Blueprint

| ID | Requirement | Complete |
|:---|---|---|
| 12 | Blueprint updates should be idempotent | Yes |
| 13 | When updating a Blueprint, I should be able to automatically increment the version | Yes |

### Azure Pipeline Build Agents

| ID | Requirement | Complete |
|:---|---|---|
| | I should be able to use Azure Pipeline hosted build agents. | Yes |
| [35]() | I should be able to use self-hosted build agents. | Yes |

### Blueprint Assignment