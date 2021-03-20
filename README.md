# PickBins Web Application
A cross platform application to manage a schedule to notify the user about the arrival time of the pick-up vehicle. Based on Node.js, Express.js, and React.js frameworks, building an application including back-end restful API, front-end web app and mobile app on cross platforms.


Deployed with complete CI/CD pipeline : integrated the pipeline first through Jenkins, provisioned the infrastructure using Terraform, automated the system task with Ansible, containerized applicaton with Docker, configured the full stack containers using Kubernetes, and finally deployed in Nginx web server.

**Technology Requirements**
  1. Git - for source code management and version control.
  2. Jenkins - to integrate the whole CI/CD pipeline of our application.
  3. Ansible - to automate the system task for the web application. 
  4. Docker - to create an image for all the required services and containerize it in a docker registry (Docker-Hub).
  5. Kubernetes - to manage the containers and deploy each of the services in Nginx server. 

**Server Requirements**
  1. [Server1] :- Jenkins and Ansible Server - where all our Jenkins job resides and Ansible can perform the system tasks.
  2. [Server2] :- Docker Host and K8S Worker Node - Docker host is where the application's client and server images are created and deployed in registry. Also, the worker node is where the k8s master deploys its services. 
  3. [Server3] :- K8S Master - where the deployment of our all services comes along. 

NOTE :- In Jenkins, you need to install Publish over SSH plugin to transfer files and to execute ansible playbooks on different servers. 

https://github.com/bipkar/Pick-Bins-Web-App/blob/main/CI:CD-Pipeline.png 
