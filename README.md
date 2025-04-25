# gd

Feature
Azure Virtual Machines
Azure Blob Storage
Azure SQL Database
Purpose
Provides IaaS – virtualized servers
Stores unstructured data (files, logs)
PaaS for relational database management
Use Case
Host applications, run OS/software
Store backups, media, documents
Store and manage relational data (SQL)
Control
Full control over OS and software
Object storage, managed by Azure
Managed database with limited admin rights
Scalability
Manual or auto-scaling VMs
Auto-scalable as per data size
Elastic scaling based on workload
Pricing
Based on usage time and resources
Based on storage and access frequency
Based on DTUs or vCores used
1. Compare and contrast Azure Virtual Machines, Azure Blob Storage, and Azure SQL Database in terms of their purpose and use cases.
 
2. Describe Azure App Service, Azure Functions, and their roles in building cloud-native applications.
• Azure App Service:
o A fully managed Platform as a Service (PaaS) for hosting web applications, RESTful APIs, and mobile backends.
o Supports multiple programming languages like .NET, Java, PHP, Python, and Node.js.
o Offers features such as automatic scaling, custom domains, and CI/CD integration.
o Ideal for running scalable and secure web applications without managing infrastructure.
• Azure Functions:
o A serverless compute service that allows you to run code on-demand in response to events (like HTTP requests, timers, queues).
o You only pay for the execution time and resources consumed.
o Best suited for microservices architecture, background tasks, and automation.
Comparison:
• App Service is for always-running web apps, while Functions are event-driven and serverless.
• Both enable faster development and deployment of applications with minimal infrastructure overhead.
 
3. Explain the role of Azure Virtual Network, Azure Security Center, and Azure Active Directory in managing and securing cloud resources.
• Azure Virtual Network (VNet):
o Allows the creation of a logically isolated network in the cloud.
o Enables secure communication between Azure resources, on-premises networks, and the internet.
o Supports features like subnets, IP address assignment, route tables, and network security groups (NSGs).
• Azure Security Center:
o A unified infrastructure security management system.
o Provides security assessments, threat protection, and compliance monitoring.
o Recommends best practices to strengthen cloud security posture.
• Azure Active Directory (Azure AD):
o A cloud-based identity and access management service.
o Enables single sign-on (SSO), multi-factor authentication (MFA), and role-based access control (RBAC).
o Helps manage users and permissions across Azure, Microsoft 365, and third-party apps.
Together, these services ensure secure connectivity, protect against threats, and manage identities/access in a cloud environment.
4. Explain the architecture and working of Azure Data Factory for implementing database operations like insert, update, and delete.
Azure Data Factory (ADF) is a cloud-based ETL (Extract, Transform, Load) and data integration service. It allows for the orchestration of data workflows between different data stores and compute services.
Architecture Components:
• Pipelines: Logical grouping of activities (e.g., Copy, Data Flow).
• Activities: Define the actual steps like Copy Activity, Data Flow Activity.
• Datasets: Point to data structures (like tables, files) used as inputs/outputs.
• Linked Services: Define the connection information for external data sources.
Working for Insert/Update/Delete:
• Use Mapping Data Flows to visually design transformation logic.
• In Data Flow:
o Source: Connect to the input data (e.g., CSV, SQL table).
o Derived Column / Conditional Split: Identify records to insert, update, or delete.
o Sink: Connect to destination SQL table and choose the appropriate upsert/delete option.
• Triggers (manual/scheduled/event-based) initiate the pipeline.
Thus, ADF supports complex database operations in a serverless and scalable environment without coding in traditional SQL.
 