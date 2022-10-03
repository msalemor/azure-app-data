# Secure Azure Solutions

Azure PaaS App and Data Reference Architecture

## Secure App Services and Azure SQL Solution

### Solution Diagram
![Solution Diagram](https://github.com/msalemor/azure-app-data/blob/main/images/secure-paas-data-app.png)
### Azure Services
- Networking
  - VNET/Subnets
  - NSGs
  - FrontDoor Premium with WAF
  - Private Endpoint (Web and SQL)
- Compute
  - App Services
- Database
  - Azure SQL
- Telemetry:
  - Application Insights
  - Log Analytics
- Identity
  - Azure AD
  - User Managed Identity

### Security
#### Networking
- Traffic is WAF ispected for attacks
- All traffic stays withing the Microsoft network. PaaS services behind Private Link. 
- NSGs open only required ports
#### Identity
- Application proted by modern identity providers via Azure Active Directory
#### Database
- Encryption in transit and at rest
- AAD integration
#### Application
- Application leverages User Managed Idenity (can connect to services without passwords)
### Scalabiltiy
#### Web App
- Can scale up or out with rules
#### Database
- Database can be scaled in and out
### Resiliency
