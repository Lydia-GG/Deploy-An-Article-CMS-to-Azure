# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

####  Azure Virtual Machines vs App Service: 


|              | Virtual Machines (VMs)                                                                                                                                                                                                          | App Service                                                                                                                                                                                                                                                                                                       |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Cost         | Provides infrastructure as a service so it is the Lower up-front cost compared to purchasing and maintaining hardware. it suits the big project.                                                                                                                                                   |There are three different tiers - Dev/Test, Production, and Isolated. Although you are always paying for the service plan even if the application is not running, it is still the better choice for lightweight applications like our CMS application. |
| Scalability  | Vertically by resizing the existing VM to a larger size with more RAM and more CPU, or to a smaller size with less RAM and less CPU, or horizontally you keep the same VM size, but you add more VM instances to the scale set.                                                                                                                           | Vertically you can scale up your pricing tier to increases or decreases resources and get more CPU, memory, disk space etc... , horizontally increases or decreases the number of Virtual Machine .       |
| Availability | Provides high availability                                        |  Provides high availability                                           
| Workflow     | They can be more time consuming for the developer than other compute options.                                                                                                                                                  | Continuous deployment model using GitHub, Azure DevOps, or any Git repo.                                                                                                                                                                                                                                          |


I chose App service for the CMS application.
### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.*   
##### why I chose app services :  

CMS application is a lightweight app and app service costs are less than VMs and provides continuous deployment. also, I want to focus more on app development and there is no need for hardware service.