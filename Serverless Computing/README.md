# Serverless Computing

Handle BackEnd scenarios

## Azure Functions

Serverless compute for several coding languages.   Stateless environment
Orchestration task    
No concern platform or Infraestructure  
Rest request  


## Azure Logic Apps
Quickly build powerful integration solutions. No code development platform. Orchestrate Workflows, and 
Start with a trigger.       

Solutions:   
    - App Integration   
    - Data Integration   
    - Enterprise Integration   
    - B2B Integration   
    - System Integration 

Gallery with more than 200 connectors


# Serverless Computing Comparison

Azure Functions  
Azure Logic Apps  

Functions and Logic Apps can both create complex orchestrations. An orchestration is a collection of functions or steps that are executed to accomplish a complex task.   

- With Functions, you write code to complete each step.   

- With Logic Apps, you use a GUI to define the actions and how they relate to one another (WorkFlow).   

Differences between functions and Logic Apps

|**Feature**|**Functions**|**Logic Apps**|
|:---:|:---:|:---:|
|State|Normally stateless, but durable Functions provide state| Stateful|
|Development|Code-first (imperative)|Designer-first (Declarative)|
|Connectivity|About a dozen built-in binding types. Write code for custom buildings|Large collection of connectors. Enterprise Integration Pack for B2B scenarios. Build custom connectors|
|Actions|Each activity is an Azure Function. Write code for activity functions|Large collection of ready-made actions|
|Monitoring|Azure Application insights|Azure portal, Log Analytics|
|Management|REST API, Visual Studio| Azure Portal, REST API, Power Shell, Visual Studio|
|Execution Context|Can run locally or in the cloud| Runs only in the cloud|