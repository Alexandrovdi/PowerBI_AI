### [Start page](https://github.com/Alexandrovdi/PowerBI_AI) 


# Setup

## Prerequisites

1. Your laptop: Windows (VM or Parallels is fine, sorry MacOS or Linux users, Power BI Desktop only runs on Windows).
1. Your Azure Subscription


## Introduction 

### Set up your development environment.

The first challenge is to setup an environment that will help you build the end to end solution.  The primary exercise here is ensuring the necessary database, storage, and Power BI capacity exist for subsequent labs.  This database can be restored either manually via the Azure Portal.  Download the [source files used for this hack](https://downgit.github.io/#/home?url=https://github.com/Alexandrovdi/PowerBI_AI/tree/main/Data).

Download these files and load them to a storage container in your Azure subscription to get started.

## Setup steps
1. Create Storage account 
2. Create Container and name it "backup"
3. Upload backup to storage.
4. Create SQL Server (logical server)
   - In Networking menu in SQL Server, we must "Allow Azure service and resources to access this server" and we must add "Add your client IP address"
5. Import database to SQL Server 
   - Use STANDART plan and 20 DTUs


## Success criteria

A restored version of the Adventure Works Data Warehouse

<br>
<br>

## Learning resources


| **Description**                            |                              **Links**                                                                       |
| ------------- | ------------- |
| create storage account  | https://docs.microsoft.com/en-us/azure/storage/common/storage-account-create?tabs=azure-portal#create-a-storage-account-1|
| create sql server   | https://docs.microsoft.com/en-us/azure/azure-sql/database/logical-servers?view=azuresql#manage-servers-databases-and-firewalls-using-the-azure-portal |
| azure sql server import db | https://docs.microsoft.com/en-us/azure/azure-sql/database/database-import?view=azuresql&tabs=azure-powershell |
| Create the new workspace in Power BI | <https://docs.microsoft.com/en-us/power-bi/service-create-the-new-workspaces> |
| Create Power BI Embedded Capacity in the Azrue Portal | https://docs.microsoft.com/en-us/power-bi/developer/embedded/azure-pbie-create-capacity?tabs=portal%2Cui#create-a-capacity |
| Delete !!!! Configure and manage capacities | <https://docs.microsoft.com/en-us/power-bi/service-admin-premium-manage> |

<br>

[Next step (Working with Data in Power BI) >](https://github.com/Alexandrovdi/PowerBI_AI/blob/main/Challenge%20steps/Step%202%20-%20Dataflows.md)
