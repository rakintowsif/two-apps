# Task-1 Solution

These are the quick steps to setup this project

Comes with [Docker](https://www.docker.com/) [Steps](#Installation) and [Local Setup Instructions](#Requirements-To-Run-Locally):
- app1,app2: `Laravel-8/PHP-8.0`
- nginx-server: `Nginx:1.10`

##### Installation (App1)
- `git clone https://github.com/towsifrakin/two-apps.git`
- `cd two-apps`
- `docker-compose up -d`
--  to run the docker container
- `docker exec -ti app1 bash`
--  to enter into the app1 container
- `cp .env.example .env && composer install && php artisan key:generate`
- `docker-compose up -d`
##### Installation from poject root directory(App2)
- `cd App_2`
- `docker-compose exec app2 composer install && cp .env.example .env && docker-compose exec app2 php artisan key:generate`

Now that all containers are up and running 

###### app1 URL- [127.0.0.1:8081](http://127.0.0.1:8081)
###### app2 URL- [127.0.0.1:8082](http://127.0.0.1:8082)


---
# Task-3 Solution

Imagine that I want to deploy an e-commerce website: 
- I want to host my website on Azure because cloud computing makes reliability, data backup, disaster recovery and business continuity easier and less expensive. It’s easy to handle as I don’t need to maintain any physical infrastructure.
- I need Azure VM for the deployment. I will use Virtual Machine Scale Sets which can create and manage a group of identical, load-balanced VMs. 
- I will use Azure DevOps as the solution should include the CI/CD pipeline.
- I will use Azure Resource Manager (ARM) which is the deployment and management service for Azure.
- Last of all, I want to use Azure Monitor which is a platform for collecting data on resources, analyzing that data, visualizing the information and even acting on the results. Azure Monitor can monitor Azure resources. 


##### Questions and Improvements

For any question or emprovement please send an e-mail to Towsif Rakin [towsifrakin1994@gmail.com]
