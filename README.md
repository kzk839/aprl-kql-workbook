# aprl-kql-workbook

This is a template of an Azure Workbooks that consolidates Azure Resource Graph for resource detection of Azure Services, which is published on [Azure Proactive Resiliency Library (APRL)](https://azure.github.io/Azure-Proactive-Resiliency-Library/services/). 

It summarizes the queries for each category and service to find resources that do not comply with the recommended practices, so that you can avoid copying and pasting queries one by one.

## Note
These books are created manually, so may lag behind the original APRL.

As of March 7, 2024 (JST), it reflects up to [PR #309](https://github.com/Azure/Azure-Proactive-Resiliency-Library/pull/309) in the original Repository

it has not been tested for all services.

- APRL_QueriesBook.workbook
  
  This workbook uses the KQL published at APRL without modification. It can only be filtered by subscription.
  
- APRL_QueriesBook_Filter.workbook
  
  This workbook is based on the KQL published at APRL, with modifications to allow for filtering.In addition to subscriptions, resource groups and tags can be used to filter.

## Screenshot
- APRL_QueriesBook.workbook

<img width="893" alt="image" src="https://github.com/kzk839/aprl-kql-workbook/assets/67820613/bcea2fce-9b07-440c-8bc0-6e7edd55e17c">



- APRL_QueriesBook_Filter.workbook

<img width="888" alt="image" src="https://github.com/kzk839/aprl-kql-workbook/assets/67820613/ef36e38e-17c2-4718-8f81-0ff8fb9d06bd">


## How to import this Workbook on your Subscription

### 1. Open Monitor and navigate to the Workbooks menu

To begin the installation process, you'll first need to access Azure Monitor from your Azure portal. Once you're in Azure Monitor, locate and click on the "Workbooks" menu on the left pane.  
On the Workbooks dashboard, you'll see a button to "+ New" a new Workbook. Click on this option to initiate the creation of a new Workbook.

![image](https://github.com/Azure/fta-postmigrationtasks/assets/3822284/d690c397-dc0a-4cec-b3ab-932fa329597d)

### 2. Import Workbook
Next, click on 'Advanced Editor' to open the editor screen. 
![image](https://github.com/Azure/fta-postmigrationtasks/assets/3822284/35ef1afb-5098-486a-8f93-35f7cdc67961)

Then paste the entire contents of the `APRL_QueriesBook.workbook` into the editor section.
Then click `Apply`.

![image](https://github.com/Azure/fta-postmigrationtasks/assets/3822284/296702b3-2c11-4323-9246-6620c6a5b23a)

Finally, press the Save button to save the Workbook as resource to the desired Resource Group.

![image](https://github.com/kzk839/aprl-kql-workbook/assets/3822284/c92644ac-74ab-4714-b2c9-2a163f044bd1)
