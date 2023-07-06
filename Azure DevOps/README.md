# Azure DevOps

## Azure Boards 
    
   Project management tool.

   With Azure Boards, teams can administrate their software projects.

   It gives a set of capabilities with native support for Scrum and Kanban.

   Offers custom control panels and integrated reports.

   Tracking of user stories, pending work, tasks, functions and bugs related with a project

   Processes:
   * Agile
   * Basic
   * Scrum
   * CMMI (Capability Maturity Model Integration)

## Azure Repos  


## Azure Pipelines

  Compila y prueba automaticamente los proyectos de codigo para ponerlos a disposicion de otros usuarios. Funciona con cualquier tipo de proyecto o lenguaje.

  Combina la integracion continua CI (Continuos Integration) y la entrega continua CD (Continuos Delivery) para probar y compilar el codigo de forma constante y coherente, y enviarlo a cualquier destino.


  1. Continuos Integration CI

    Es la practica utilizada por los equipos de desarrollo para automatizar la combinacion (compilacion, build) y las pruebas de codigo.

    La implementacion de CI ayuda a detectar errores al principio del ciclo de desarrollo , lo que hace que sean menos caros de corregir.

    LAs pruebas automatizadas se ejecutan como parte del proceso de CI para garantizar la calidad.

    Los artefactos se generan a partir de sistemas de CI y se alimentan a los procesos de lanzamiento para impulsar implementaciones frecuentes.


  2. Continuos Delivery
    
    Es un proceso por el cual se crea, prueba e implementa codigo en uno o varios entornos de prueba y produccion.

    La implementacion y prueba en varios entornos impulsa la calidad.

    Los sistemas de CI producen los artefactos que en el delivery se pueden implementar, incluidas la infraestructura y las aplicaciones.

    Los sistemas de supervision y alerta se ejecutan continuamente para impulsar la visibilidad en todo el proceso de CD.



## Azure Test Plans  


## Azure Artifacts  



## Azure DevTest Labs

# Main Definitions

## Agents

To build your code or deploy your software using Azure Pipelines, you need at least one agent. As you add more code and people, you'll eventually need more.
When your pipeline runs, the system begins one or more jobs. An agent is computing infrastructure with installed agent software that runs one job at a time.
Jobs can be run directly on the host machine of the agent or in a container.

There are two types of agents:

### Microsoft-hosted agents  

If your pipelines are in Azure Pipelines, then you've got a convenient option to run your jobs using a Microsoft-hosted agent. With Microsoft-hosted agents, maintenance and upgrades are taken care of for you. Each time you run a pipeline, you get a fresh virtual machine for each job in the pipeline. The virtual machine is discarded after one job (which means any change that a job makes to the virtual machine file system, such as checking out code, will be unavailable to the next job). Microsoft-hosted agents can run jobs directly on the VM or in a container.

Azure Pipelines provides a predefined agent pool named Azure Pipelines with Microsoft-hosted agents.

For many teams this is the simplest way to run your jobs. You can try it first and see if it works for your build or deployment. If not, you can use a self-hosted agent.

### Self-hosted agents  

An agent that you set up and manage on your own to run jobs is a self-hosted agent. You can use self-hosted agents in Azure Pipelines or Azure DevOps Server, formerly named Team Foundation Server (TFS). Self-hosted agents give you more control to install dependent software needed for your builds and deployments. Also, machine-level caches and configuration persist from run to run, which can boost speed.

> **_NOTE:_**  Although multiple agents can be installed per machine, we strongly suggest to only install one agent per machine. Installing two or more agents may adversely affect performance and the result of your pipelines.

### Azure Virtual Machine Scale Set agents

Azure Virtual Machine Scale Set agents are a form of self-hosted agents that can be auto-scaled to meet your demands. This elasticity reduces your need to run dedicated agents all the time. Unlike Microsoft-hosted agents, you have flexibility over the size and the image of machines on which agents run.

You specify a Virtual Machine Scale Set, a number of agents to keep on standby, a maximum number of virtual machines in the scale set, and Azure Pipelines manages the scaling of your agents for you.

For more information, see Azure Virtual Machine Scale Set agents.

## Parallel jobs

Parallel jobs represents the number of jobs you can run at the same time in your organization. If your organization has a single parallel job, you can run a single job at a time in your organization, with any additional concurrent jobs being queued until the first job completes. To run two jobs at the same time, you need two parallel jobs. In Azure Pipelines, you can run parallel jobs on Microsoft-hosted infrastructure or on your own (self-hosted) infrastructure.

Microsoft provides a free tier of service by default in every organization that includes at least one parallel job. Depending on the number of concurrent pipelines you need to run, you might need more parallel jobs to use multiple Microsoft-hosted or self-hosted agents at the same time. For more information on parallel jobs and different free tiers of service, see Parallel jobs in Azure Pipelines.







