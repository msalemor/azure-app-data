# azure-app-data
Azure PaaS App and Data Reference Architecture

## Secure Solution

### Solution Diagram
### Security
#### Networking
- Traffic is WAF ispected for attacks
- PaaS Service with Private Link. All traffic stays withing the Microsoft network
- NSG open only required ports
#### Identity
- Application proted by modern identity providers
#### Database
- Encryption in transit and at rest
- AAD integration
#### Application
- Application leverage User Manage Idenity (can connect to services without passwords)
### Scalabiltiy
#### Web App
- Can scale up or out with rules
### Resiliency
