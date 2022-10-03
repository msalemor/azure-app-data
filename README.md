# azure-app-data
Azure PaaS App and Data Reference Architecture

## Secure Solution

### Solution Diagram
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
- Application leverages User Manage Idenity (can connect to services without passwords)
### Scalabiltiy
#### Web App
- Can scale up or out with rules
### Resiliency
