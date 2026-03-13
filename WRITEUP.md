# Write-up

## Analyze, choose, and justify the appropriate resource option for deploying the app

### Option 1: Virtual Machine (VM)

A Virtual Machine provides full control over the operating system and environment. With a VM, the developer must install and manage the web server, Python runtime, security updates, and scaling configuration. While this offers flexibility and control, it requires more maintenance and operational effort. Monitoring, updates, and scaling would need to be configured manually.

### Option 2: Azure App Service

Azure App Service is a Platform-as-a-Service (PaaS) offering that allows developers to deploy web applications without managing the underlying infrastructure. It automatically handles server maintenance, scaling, security patches, and integration with other Azure services such as Azure SQL Database and Azure Storage. App Service also provides built-in logging, monitoring, and deployment integration with GitHub.

### Chosen Deployment Option

For this project, Azure App Service was chosen as the deployment option. App Service simplifies the deployment process and removes the need to manage servers manually. It also integrates easily with Azure SQL Database and Azure Blob Storage, which are required components of this project. Additionally, App Service provides built-in monitoring and logging tools that help track application performance and troubleshoot issues.

## Assess app changes that would change your decision

If the application required greater control over the operating system, custom networking configurations, or specialized software dependencies, a Virtual Machine might become the better option. For example, if the application needed custom background services, advanced system-level configuration, or non-supported runtime environments, deploying on a VM would provide the flexibility required. However, for a standard web application like the Article CMS, Azure App Service remains the more efficient and scalable choice.
