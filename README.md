# PickBins Web Application
A cross platform application to manage a schedule to notify the user about the arrival time of the pick-up vehicle. Based on Node.js, Express.js, and React.js frameworks, building an application including back-end restful API, front-end web app and mobile app on cross platforms.


Deployed with complete CI/CD pipeline : integrated the pipeline first through Jenkins, provisioned the infrastructure using Terraform, automated the system task with Ansible, containerized applicaton with Docker, configured the full stack containers using Kubernetes, and finally deployed in Nginx web server.

**Technology Requirements**
  1. AWS - Amazon Web Services as server provider and networking. 
  2. Git - for source code management and version control.
  3. Jenkins - to integrate the whole CI/CD pipeline of our application.
  4. Ansible - to automate the system task for the web application. 
  5. Docker - to create an image for all the required services and containerize it in a docker registry (Docker-Hub).
  6. Kubernetes - to manage the containers and deploy each of the services in Nginx server. 

**Server Requirements**
  1. [Server1] :- Jenkins and Ansible Server - where all our Jenkins job resides and Ansible can perform the system tasks.
  2. [Server2] :- Docker Host and K8S Worker Node - Docker host is where the application's client and server images are created and deployed in registry. Also, the worker node is where the k8s master deploys its services. 
  3. [Server3] :- K8S Master - where the deployment of our all services comes along. 

NOTE :- In Jenkins, you need to install **Publish over SSH** plugin to transfer files and to execute ansible playbooks on different servers. 


# CI/CD Pipeline
   <img width="722" alt="CI:CD-Pipeline" src="https://user-images.githubusercontent.com/56852163/111853319-7fa14e00-88e8-11eb-8c4c-d3434a427b19.png">

