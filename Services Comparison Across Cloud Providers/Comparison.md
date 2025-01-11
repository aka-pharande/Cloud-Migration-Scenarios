# Cloud Resource Comparison Across AWS, Azure, and Google Cloud

| #  | Description                                                                 | AWS Service Name                | Azure Service Name                 | Google Cloud Service Name      |
|----|-----------------------------------------------------------------------------|---------------------------------|------------------------------------|--------------------------------|
| 1  | A compute service that provides scalable virtual machines for running applications. | EC2 (Elastic Compute Cloud)    | Virtual Machines                   | Google Compute Engine                 |
| 2  | An object storage service used to store and retrieve data, commonly used for backups and static website content. | S3 (Simple Storage Service)     | Blob Storage                       | Cloud Storage                  |
| 3  | A managed relational database service that supports multiple database engines like MySQL, PostgreSQL, and SQL Server. | RDS (Relational Database Service)| Azure SQL Database   | Cloud SQL                      |
| 4  | A serverless compute service that allows you to run code in response to events without provisioning or managing servers. | Lambda                          | Azure Functions                    | Cloud Functions                |
| 5  | A virtual private network service that allows you to create isolated networks within the cloud provider's infrastructure. | Amazon VPC (Virtual Private Cloud)     | Azure Virtual Network (VNET)              | VPC (Virtual Private Cloud)    |
| 6  | A content delivery network (CDN) service that delivers data, videos, applications, and APIs to customers around the world with low latency. | CloudFront                      | Azure CDN                         | Cloud CDN                      |
| 7  | A managed NoSQL database service designed for low-latency, high-scale applications. | DynamoDB                        | Cosmos DB                         | Firestore                      |
| 8  | A block storage service for use with virtual machines, offering persistent storage for data. | EBS (Elastic Block Store)       | Azure Disk Storage                 | Persistent Disk                |
| 9  | A managed container orchestration service based on Kubernetes.              | EKS (Elastic Kubernetes Service) | Azure Kubernetes Service (AKS)    | GKE (Google Kubernetes Engine) |
| 10 | A service for managing user access and encryption keys to secure cloud resources. | IAM (Identity and Access Management) | Microsoft Entra ID             | Cloud IAM                     |
| 11 | A platform that automates application deployment and scaling without needing to manage infrastructure. | AWS Elastic Beanstalk                     | Azure App Service                  | Cloud Run                      |
| 12 | A service that provides monitoring and logging of applications and infrastructure, offering insights into resource usage and performance. | CloudWatch                      | Azure Monitor                      | Cloud Monitoring               |
| 13 | A domain name system (DNS) service that routes traffic globally and translates domain names to IP addresses. | Route 53                        | Azure DNS                          | Cloud DNS                     |
| 14 | A load balancing service that distributes incoming network traffic across multiple targets, improving application availability. | ELB (Elastic Load Balancing)    | Azure Load Balancer                | Cloud Load Balancing          |
| 15 | A service that automatically scales your cloud infrastructure based on demand, ensuring resources are available as needed. | EC2 Auto Scaling                | Virtual Machine Scale Sets         | Managed Instance Groups        |
| 16 | A message queuing service that enables applications to send and receive messages between different components. | SQS (Simple Queue Service)      | Azure Queue Storage                | Cloud Pub/Sub                 |
| 17 | A managed real-time data streaming service that collects and processes large amounts of data from various sources. | Amazon Kinesis Data Streams                       | Azure Stream Analytics             | Cloud Pub/Sub                 |
| 18 | A fully managed, highly scalable data warehouse service optimized for analytics and large-scale queries. | Redshift                        | Azure Synapse Analytics            | BigQuery                      |
| 19 | A service that automates the execution of workflows and allows the integration of different cloud services in a sequence of steps. | Step Functions                  | Azure Logic Apps                   | Cloud Functions                |
| 20 | A service that integrates multiple data sources and enables data migration, transformation, and movement across platforms. | AWS Glue                        | Azure Data Factory                 | Cloud Data Fusion              |
| 21 | A data catalog and governance service that helps manage metadata across your data estate, supporting compliance and security. | AWS Glue Data Catalog           | Azure Data Catalog                 | Data Catalog                   |
| 22 | A set of machine learning and AI services that provide pre-built models, APIs, and tools for developers to easily implement AI in their apps. | SageMaker                       | Azure Machine Learning             | AI Platform                    |
| 23 | A service that allows you to define and deploy infrastructure using code, automating the management of cloud resources. | CloudFormation                  | Azure Resource Manager             | Cloud Deployment Manager       |
| 24 | A fully managed CI/CD service that automates the building, testing, and deployment of applications to production environments. | CodePipeline                    | Azure DevOps                       | Cloud Build                    |
| 25 | A desktop as a service (DaaS) offering that allows you to deploy virtual desktops in the cloud and access them remotely. | Amazon WorkSpaces               | Azure Virtual Desktop              | Citrix Virtual Apps and Desktops                       |
| 26 | A backup and disaster recovery service that helps to protect your data by creating backups and replicas of your cloud resources. | AWS Backup                      | Azure Backup                       | Google-managed Backup and DR Service           |
| 27 | A service designed for big data analytics, allowing organizations to store, process, and analyze large datasets in real time. | EMR (Elastic MapReduce)         | Azure HDInsight                    | BigQuery                      |
| 28 | A file storage service for storing and sharing files with users, typically used in shared file systems across applications. | EFS (Elastic File System)       | Azure Files                        | Filestore                      |
| 29 | A service that helps you transcode, process, and stream media content such as video and audio. | AWS Elemental MediaConvert      | Azure Media Services               | Transcoder API                 |
| 30 | A real-time communication service used for sending notifications, emails, and text messages to users and devices. | SNS (Simple Notification Service)| Service Bus            | Cloud Pub/Sub                 |

# Introduction
AWS, Azure, and GCP are the top three cloud service providers, each with its own set of fundamental offerings and some key distinguishing features. AWS is the leading cloud service provider. Azure is second on the list and GCP is third and is steadily growing. 

# Key Similarities
These three cloud service providers have a lot in common. They all have essential services like computing, databases, storage, and networking, which have almost identical features: 

**Compute Services:** In terms of compute power, all the three cloud service providers offer the capability to spin up virtual machines that are scalable, flexible and offer a variety of SKUs to select from based on our needs. Although they perform the same functions, in each service provider they are named differently. For example, AWS has Elastic compute cloud (EC2), Azure has Virtual Machines, and Google has Compute Engine. 

**Object Storage:** All the three cloud providers offer capability to store large amounts of unstructured data in a secure and reliable environment. These storage offerings offer additional features such as life cycle management for cost efficiency, backup and data encryption. For example, AWS has S3, Azure has blob storage and Google has cloud storage. 

**Database Services:** The database services offered in the three cloud providers are pretty much similar. They all offer the capability to store relational and non relational data. This is a PaaS offering which is scalable, secure and fully managed. For non relational database, AWS has DynamoDB, Azure has Cosmos DB, and GCP has Fire store. 

**Networking Services:**  They all provide highly advanced networking services to protect the cloud infrastructure. These services enable secure communication from one resource to another. The virtual isolated separate networks are called Amazon VPC in AWS, VNET in Azure and Cloud VPC in Google cloud. 

# Key Differences
They have a lot in common, but they also have significant differences.

**Machine Learning and AI Services** that the three platforms offer differ a great deal in the capabilities they offer. For instance, AWS provides the service Amazon SageMaker, which is intended for building machine learning models. The Azure platform offers Azure Machine Learning, which is better suited for those who want to use Microsoft ecosystem and work along the lines of “low-code” or “no-code” directions. On the other hand, Google Cloud AI has, arguably, the strongest features for the user who enjoys working with natural language processing or computer vision models and favors a more “customized” experience.

**Networking and Content Delivery:** AWS offers Amazon CloudFront (a global content delivery network with an impressive customer worldwide), and AWS Direct Connect (a private network linked point of entry into the AWS Cloud). Azure provides its own CDN (which caches data at edge locations worldwide to deliver content quickly), and ExpressRoute (a physical network for private connections to the cloud). Google Cloud’s CDN works well with their geographically distributed infrastructure that ensures content is delivered in time for the customers within regions.

**Data Warehousing:** AWS has Amazon Redshift, which is fast, due to its column-store architecture, offering great compression. While Azure has Azure Synapse Analytics, combining the ideas of big data with data warehousing, supporting batch and real-time analytics. GCP is different and offers BigQuery, a serverless data warehouse that eases querying and analysis, and reduces maintenance, which is good for data analysis.


# Unique features
**AWS** offers more than 200 services – including Amazon SageMaker for machine learning. AWS Lambda, a serverless compute platform with which you can run code without managing servers – which makes it very agile and fits well with most businesses. AWS connects well with external services.

**Azure** is a good choice for many companies that want to use cloud services but also integrate them with what they already have on premises. Using Azure Arc, which connects their on prem infrastructure to the cloud set up and Azure Site Recovery (ASR), which enables instant recovery in case of issues. Microsoft products such as Office 365 are also a big reason for people to choose Azure. Microsoft takes security very seriously. Security is one of the most essential elements and so Azure offers many tools for security, including Azure Security Center.

**Google Cloud Platform** (GCP) has the most compelling argument when it comes to data analytics and AI. Its BigQuery is unparalleled for fast SQL queries and real-time, in-house analytics. GCP also has solid machine learning baked into various services, such as AutoML and TensorFlow that allow companies to make their own models. Google’s global network helps keep things quick, which is perfect for apps needing fast responses, like gaming.


# Naming conventions
Each service provider has their own naming conventions for similar services. AWS is known for using acronyms to name many of its services. For examples, EC2 for Elastic Compute Cloud, S3 for Simple Storage Service, etc. Whereas Azure tends to use descriptive and straightforward terms for its services, making them intuitive and easy to understand. For instance, virtual machine, blob storage, etc. Google cloud also uses descriptive names for its services similar to azure. Their services usually have the prefix “Cloud” in most of their offerings. For example, Cloud functions and Cloud Firestore. 
