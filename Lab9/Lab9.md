# 1. Cost Estimate Report

The GCP pricing calculator was used to generate this cost report. Here's a link to a [pricing estimate](https://cloud.google.com/products/calculator/?hl=en&dl=CjhDaVE1WmpsaFl6RTRNeTAyWkRRekxUUmhaR0V0T1dFM05pMDVNek5oTkRZeU9UUmhaakVRQVE9PRAIGiREMzQ4QTdFQy0yMzc0LTQ4RUItQTg1Ny00QkMzOUVERkI5RDY). 

## 1.1 Operational Cost Estimation
### Web Front-End Cluster
- **Virtual machines:** 10 virtual machines will be deployed accross three regions: US-Central, Europe-London, and Mumbai.
Following is the detialed cost breakdown for each region along with the different pricing models.

| Region        | Pay-As-You-Go        | Sustained Use Discount | 1-Year Commitment   | 3-Year Commitment   |
|---------------|----------------------|-------------------------|---------------------|---------------------|
| US-Central    | $1,696.99/month      | $1,280.09/month        | $1,072.77/month     | $769.19/month       |
| Europe-London | $2,158.97/month      | $1,622.88/month        | $1,363.50/month     | $977.39/month       |
| Mumbai        | $2,037.86/month      | $1,538.10/month        | $1,288.17/month     | $923.64/month       |

- **Load Balancer:** The cost for the load balancer is the same i.e. $19.85/month for all the three region.
- **Content Delivery Network (CDN):** $27.82/month in the US, $27.82/month in Europe, and $32.86/month in Mumbai.
- **Static IP Addresses:** $7.29/month in the US, $8.75/month in Europe and Mumbai.

### API Back-End Services
- **Virtual machines:** 20 virtual machines will be required to support 50 microservices for the API 
Back-End services. Below is the table that provides a breakdown of the monthly costs for each region based on 
pay-as-you-go, sustained use discounts, and committed use discount options.

| Region        | Pay-As-You-Go        | Sustained Use Discount | 1-Year Commitment   | 3-Year Commitment   |
|---------------|----------------------|-------------------------|---------------------|---------------------|
| US-Central    | $2,793.99/month      | $1,961.79/month        | $1,767.55/month     | $1,268.37/month     |
| Europe-London | $3,597.93/month      | $2,525.75/month        | $2,273.41/month     | $1,630.79/month     |
| Mumbai        | $3,355.72/month      | $2,356.20/month        | $2,122.74/month     | $1,523.27/month     |

### Payment Processing

- **Virtual machines:** 2 virtual machines will be required per region to securely handle customer payment data. 
These VMs will be configured to meet PCI complaince and provide data encryption at transit and at rest. 
The table below provides the monthly pricing for the VMs.


| Region        | Pay-As-You-Go        | Sustained Use Discount | 1-Year Commitment   | 3-Year Commitment   |
|---------------|----------------------|-------------------------|---------------------|---------------------|
| US-Central    | $279.40/month        | $196.18/month          | $176.75/month       | $126.84/month       |
| Europe-London | $359.79/month        | $252.58/month          | $227.34/month       | $163.08/month       |
| Mumbai        | $335.57/month        | $235.62/month          | $212.27/month       | $152.33/month       |

### Database Layer
- **Primary Database (Cloud SQL):** The Cloud SQL database will be used to store 5 TB of critical operational data.
The table below demonstrates the pricing for standard and high-availability configurations across different regions, with options for pay-as-you-go and committed use discounts.

| Region        | Standard (Pay-As-You-Go) | 1-Year Commitment  | 3-Year Commitment  | High Availability (Pay-As-You-Go) | High Availability (1-Year) | High Availability (3-Year) |
|---------------|--------------------------|---------------------|--------------------|-----------------------------------|-----------------------------|-----------------------------|
| US-Central    | $948.62/month            | $923.97/month      | $897.34/month      | $1,897.25/month                   | $1,847.93/month            | $1,794.68/month            |
| Europe-London | $1,138.41/month          | $1,108.80/month    | $1,076.83/month    | $2,276.67/month                   | $2,217.50/month            | $2,153.60/month            |
| Mumbai        | $1,138.41/month          | $1,108.80/month    | $1,076.83/month    | $2,276.67/month                   | $2,217.50/month            | $2,153.60/month            |

- **Analytics Database (Bigtable):** Bigtable will be used to store 10 TB of NoSQL data for analytics purposes.
The table below provides a breakdown of the pricing.

| Region        | Pay-As-You-Go (None) | 1-Year Commitment  | 3-Year Commitment  |
|---------------|----------------------|---------------------|--------------------|
| US-Central    | $1,344.90/month      | $1,075.92/month    | $806.94/month      |
| Europe-London | $1,593.40/month      | $1,274.72/month    | $956.04/month      |
| Mumbai        | $1,549.56/month      | $1,239.65/month    | $929.74/month      |

- **Data Warehouse (BigQuery):** BigQuery will be used to store 15 TB of data for reporting and machine learning purposes.
 The table below outlines the pricing for different regions, including pay-as-you-go and committed use options.

 | Region        | Pay-As-You-Go (None) | 1-Year Commitment  | 3-Year Commitment  |
|---------------|----------------------|---------------------|--------------------|
| US-Central    | $6,923.05/month      | $6,047.05/month    | $5,171.05/month    |
| Europe-London | $8,894.05/month      | $7,755.25/month    | $6,616.45/month    |
| Mumbai        | $7,908.55/month      | $6,901.15/month    | $5,893.75/month    |

### Data Analytics and ML Processing
- **Compute Engine:** 10 GPU-enabled VMs will be allocated for machine learning model training and efficient processing of complex algorithms. 
The table below provides the pricing details for different regions.

| Region        | Pay-As-You-Go (None) | 1-Year Commitment  | 3-Year Commitment  |
|---------------|----------------------|---------------------|--------------------|
| US-Central    | $3,951.99/month      | $2,489.77/month    | $1,802.19/month    |
| Europe-London | $4,090.75/month      | $2,577.18/month    | $1,864.54/month    |
| Mumbai        | $4,670.86/month      | $2,959.37/month    | $2,075.64/month    |

### Backup and Disaster Recovery
As per the [Google Cloud SQL pricing documentation](https://cloud.google.com/sql/pricing?utm_source=google&utm_medium=cpc&utm_campaign=na-CA-all-en-dr-bkws-all-all-trial-e-dr-1707554&utm_content=text-ad-none-any-DEV_c-CRE_678241001166-ADGP_Hybrid%20%7C%20BKWS%20-%20MIX%20%7C%20Txt-Databases-Cloud%20SQL%20Pricing-KWID_43700077224547317-kwd-353549069658&utm_term=KW_gcp%20cloud%20sql%20pricing-ST_gcp%20cloud%20sql%20pricing&gad_source=1&gclid=CjwKCAjw-JG5BhBZEiwAt7JR615_hZoJ-ZZULWIA8gcbQWncXtQ--4WaZPh68MzflnPCQ0gMzG3pmhoCmwUQAvD_BwE&gclsrc=aw.ds), read replicas and failover replicas in Google Cloud SQL are charged at the same rate as standalone instances. This means that if you replicate a database in another region, the cost will be approximately double the cost of the databases listed above.

## 1.2 Management and Monitoring Costs
- **Cloud Monitoring:** Estimated at $7,701.30/month to monitor all VMs, databases, and other services.
- **Cloud Logging:** With a logging retention duration of 6 months and 300 GiB/month of storage, the cost is approximately $143.00/month.
- **Trace Spans and Uptime Checks:** Estimated at $488.40/month for 5-minute intervals across all regions.

## 1.3 Migration Cost Estimation
The migration costs are a one time expenditure required for data transfer, database replication, and temporary migration
resources. In fact, if the migration is homogenous i.e. where the source and destination are on the same database engine, it wouldn't cost anything at all.
However, if it ends up being a hetrogenous move, it will cost $0.463/GB to backfill the data. 
Given we have to migrate 30 TB of data, in thw worst case (heterogenous move), we will incur a one time cost of $14223.36 to migrate the data to Cloud databases.
More information of the database migration service pricing can be found [here](https://cloud.google.com/database-migration/pricing).

# 2. Cost Optimization Strategy
**Reserved Instances vs. Pay-As-You-Go** 
- With a 1-year or 3-year commitment, ShopPro can significantly reduce costs across multiple components.
- Web Front-End Cluster: Savings range from ~40% with a 1-year commitment to over 55% with a 3-year commitment.
- API Back-End Services: Using reserved instances for a 1-year or 3-year commitment saves ~30-40%.

The table below highlights monthly cost differences for a sample component, comparing pay-as-you-go with 1-year and 3-year commitment discounts.

| Component              | Region        | Pay-As-You-Go | 1-Year Commitment | 3-Year Commitment |
|-----------------------|---------------|----------------|-------------------|-------------------|
| Web Front-End VMs     | US-central    | $1,696.99      | $1,072.77         | $769.19           |
| API Back-End VMs      | Europe-west2  | $3,597.93      | $2,273.41         | $1,630.79         |
| Database (SQL)        | Asia-south1   | $1,138.41      | $1,108.80         | $1,076.83         |


**Right-Sizing and Auto-Scaling**
- Implementing auto-scaling policies for the API back-end and front-end clusters can minimize costs during off-peak times while maintaining performance during peak traffic.
- Right-sizing VMs based on performance metrics and scaling requirements is recommended to avoid over-provisioning and excess spending.

**Hybrid Benefits**
- Leveraging hybrid benefits for existing software licenses where applicable (e.g., Windows Server) can further reduce monthly costs.

# 3. Future Growth and Budget Plan
## 3-Year Cost Projection and Adjustments

### Projected Growth
A 10-15% increase in usage each year can be expected. Which means that more virtual machines, databases, and storage will be needed, which will increase the costs.

### Strategic Adjustments
- **Newer Instance Types**: Upgrade to the latest, more cost-effective virtual machines to save money.
- **Serverless Services**: Move some non-critical tasks to serverless solutions to lower the computing costs.
- **Multi-Year Commitments**: Where possible, extend the commitments to 3 years to save even more on costs.
