# Protecting Security Threats 

### Azure Security Center

- Monitor Security Setting   
- Automatically Apply security settings   
- Provide Security Recommendations   
- Continuosly Monitor your resources   
- Use Machine Learning to prevent malware  
- Detect inbound Attacks   
- Just in time access control   

Secure score: (percent %)
- High
- Medium 
- Low

1. Secure posture report   
2. Improve your security poster    
3. Benchmark capture and KPIs


### Azure Sentinel

Security Information and Event Management (**SIEM**)

1. Collect cloud Data at scale   
2. Detect threats, minimizing false positives      
3. Investigate Threats with AI     
4. Respond to incidents rapidly   

Use connectors:  
- Connect Microsoft Solutions    
- Connect other services ans solutions    
- Connect industry standard data sources  


### Azure Key-Vault (secrets)

Store and Manage Secrets (sensitive information).

- Manage Secrets (tokens, password, certificates, API keys)
- Manage encryption keys
- Manage SSL/TLS certificates
- Store secrets backed by hardware security modules  (HSMs)

Benefits:
- Centralized application secrets    
- Securely stored secrets and keys     
- Access monitoring and access control   
- Simplified administration of application secrets    
- Integration with other Azure Services   

In practice, there are several ways to add secrets to and read secrets from Key Vault. You can use the Azure portal, the Azure CLI, or Azure PowerShell. 

    $ az keyvault secret show --name MyPassword --vault-name my-keyvault-NNN --query value --output tsv


### Azure dedicated Host

A dedicated host is a solution to regulatory compliance that requires some organizations to be the only customer using the physical machine that hosts their virtual machines. 
