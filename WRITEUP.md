Analyze, choose, and justify the appropriate resource option for deploying the app

| Tables        | Azure VM           | Azure App Service  |
| :-------------: |:-------------:| :-----:|
| Cost      | More expensive | Cheaper for basic |
|       | A1 v2      |   B1 |
|       | vCPUs: 1   |   100 total ACU |
|       | 2 GB RAM      |   1.75 GB RAM |
|  | 10 GB Temporary |    10 GB Storage |
|  | Average per month: 47.45 USD/Month      |    Average per month: 32.12 USD/Month |
| Scalability |   Scale limit: Platform image: 1000 nodes per scale set<br />Custom image: 600 nodes per scale set  |    Scale limit: Up to 30 instances,100 with App Service Environment.<br /> Vertical scaling, without having to redeploy. |
| Availability |   Virtual Machine Connectivity of at least 95%.    |    99.95% available is the least. <br />No SLA is provided for Apps under either the Free or Shared tiers. |
|   Workflow    | Deploying on a virtual machine requires many operations, and each deployment has to repeat some of the previous operations, contributing to slow application updates.     |   Deploying a CMS application on App Service with github makes app updates quick and requires only one-time configuration |
* I chose the Application Service solution to deploy the application because of its low cost, not much care about the infrastructure but focused on the application, easy   to deploy the application

Assess app changes that would change your decision:
   - An increase in the number of users
   - Need to use dedicated servers
   - Focus on improving the performance of the application
   
URL: https://flaskwebstudy.azurewebsites.net
