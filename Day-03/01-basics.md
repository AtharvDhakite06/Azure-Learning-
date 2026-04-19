# Azure Resources

A Resource in Azure is any individual service or component that you create and use.

Azure resources are the building blocks of your cloud infrastructure in Microsoft Azure. These resources can be virtual machines, databases, storage accounts, or any other service offered by Azure. Each resource is a manageable item in Azure, and they are provisioned and managed individually.

Resource manager is responsible for creating the resources 

if we r using a azure service like (vm..) so A resource is an instance of a service of ( vm or any other service )

Workflow of a resource creation 
<img width="1029" height="480" alt="image" src="https://github.com/user-attachments/assets/bc1c254b-8ae1-4683-980a-e6d1642a4fc7" />




## Resource Groups in Azure


A **Resource Group** in Azure is a logical container for resources that share the same lifecycle, permissions, and policies. 
It helps you organize and manage related Azure resources efficiently. Resources within a group can be deployed, updated, and deleted together as a single management unit.

A Resource Group (RG) is a logical container that holds related Azure resources. (by using naming convention)
reason to use :
1. manadatory in azure
2. adds capabilities such i can manage access control,policies,many....

we can control the access control (IAM) who has access who has assigned role and everything....

<img width="1010" height="439" alt="image" src="https://github.com/user-attachments/assets/3a0937b3-ab06-46d7-a889-2684394fdef0" />

We can use all access control, permission, security, Auditing, Cost...in Resource Group
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/10d72d8c-2bbd-40da-82dc-4bf69539cd10" />
<img width="1919" height="1075" alt="image" src="https://github.com/user-attachments/assets/5eaa0279-6c31-4cb9-9aed-767df0fd2cfc" />

**Interview Que**
**How to group this resources**/**How are you managing the azure resources**
(Naming Convention) for large org multiple azure accounts 

We are using resource group as per the project where we are using the one rg for payment, transactions and like that......... and using this resource groups we manage monitoring , access , network , locking , security aspects etc...

It depends on organization acc for different environment like dev,Quality assuarance, payment, transaction, production team so according to that we can create different resource group 

**For small Organization** single Azure account 
We Create 1 Rg projectname - environment ( Payment - Dev )


_**A resource and resource group is 1:1 means a VM is part of 1 resource group then it cannot be a part of the another resource group **_


### Key Points about Resource Groups:

- **Lifecycle Management:** Resources within a group can be managed collectively, making it easy to handle deployments, updates, and deletions.

- **Resource Organization:** Grouping resources based on projects, environments, or applications helps keep your Azure environment well-organized.

- **Role-Based Access Control (RBAC):** Permissions and access control are applied at the resource group level, allowing you to manage who can access and modify resources within a group.

## Azure Resource Manager (ARM) Overview

**Azure Resource Manager (ARM)** is the deployment and management service for Azure. It provides a consistent management layer that enables you to deploy resources with declarative templates. ARM templates describe the resources you need and their configurations, allowing you to deploy and update resources in a predictable manner.

### Key Features of Azure Resource Manager:

- **Template-Based Deployment:** ARM uses JSON templates to define the infrastructure and configuration of your Azure resources. This enables repeatable and consistent deployments.

- **Dependency Management:** ARM automatically handles dependencies between resources, ensuring they are deployed in the correct order.

- **Rollback and Roll-forward:** In case of deployment failures, ARM can automatically roll back changes to maintain the desired state, or roll forward to the last known good state.

- **Tagging and Categorization:** You can use tags to label and categorize resources, making it easier to manage and organize your Azure environment.

**Note:** Understanding Azure resources, resource groups, and Azure Resource Manager is fundamental to effectively utilize and manage your resources in the Azure cloud.

