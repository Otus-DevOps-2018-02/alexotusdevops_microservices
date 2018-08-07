# alexotusdevops_microservices
alexotusdevops microservices repository

##### [Homework 13](#hw13) 
 * [Main task](#hw131)  
 * [Task *](#hw132) 
##### [Homework 14](#hw14)  
 * [Main task](#hw141)  
##### [Homework 15](#hw15)  
 * [Main task](#hw151)  
 * [Task *](#hw152)  
##### [Homework 16](#hw16)  
 * [Main task](#hw161)  
##### [Homework 17](#hw17)  
 * [Main task](#hw171)  
##### [Homework 18](#hw18)  
 * [Main task](#hw181)  
##### [Homework 19](#hw19)  
 * [Main task](#hw191)  
##### [Homework 20](#hw20)  
 * [Main task](#hw201)  
##### [Homework 21](#hw21)  
 * [Main task](#hw211)  
##### [Homework 22](#hw22)  
 * [Main task](#hw221)  
##### [Homework 23](#hw23)  
 * [Main task](#hw231)  
##### [Homework 24](#hw24)  
 * [Main task](#hw241)  
##### [Homework 25](#hw25)  
 * [Main task](#hw251)  



<a name="hw13"></a>
## Homework 13
<a name="hw131"></a>
##### Main task  
  - Install docker  
  - Test primary docker commands  
  - Make images and run containers  

<a name="hw132"></a>
##### Task *  
  - Add information about images and containers in ./docker-monolith/docker-1.log

<a name="hw14"></a>
## Homework 14
<a name="hw141"></a>
##### Main task  
  - New GCP Project created  
  - Install & configure Docker-machine  
  - Create docker image and upload to hub.docker.com  
  - Test image in GCP and at local docker  


<a name="hw15"></a>
## Homework 15
<a name="hw151"></a>
##### Main task  
  - Tried to install Hadolint. After 3 unsuccessful attempts I use  
    > docker run --rm -i hadolint/hadolint < Dockerfile  
  - Create images to deploy app in docker  
  - Create Bridge network  
  - Attach docker volume 

<a name="hw152"></a>
##### Task *  
  - Run containers with new network aliases  
    > docker run -d --network=reddit --network-alias=post_db_new --network-alias=comment_db_new mongo:latest  
    > docker run --env POST_DATABASE_HOST=post_db_new --env POST_DATABASE=posts_new -d --network=reddit --network-alias=post_new alexotusdevops/post:1.0  
    > docker run --env COMMENT_DATABASE_HOST=comment_db_new --env COMMENT_DATABASE=comments_new -d --network=reddit --network-alias=comment_new alexotusdevops/comment:1.0  
    > docker run --env COMMENT_SERVICE_HOST=comment_new --env POST_SERVICE_HOST=post_new -d --network=reddit -p 9292:9292 alexotusdevops/ui:1.0  

<a name="hw16"></a>
## Homework 16
<a name="hw161"></a>
##### Main task  
  - Install docker-compose  
  - Run docker with different networks (none, brigde, host)  
  - Divide networks into front & back  
  - Docker-compose.yml edited to work with multiple networks  

<a name="hw17"></a>
## Homework 17
<a name="hw171"></a>
##### Main task  
  - New host created in GCP  
  - Install Omnibus Gitlab  
  - Customized GitlabCI  

<a name="hw18"></a>
## Homework 18
<a name="hw181"></a>
##### Main task  
  - Create new Gitlab project  
  - Share runner to new project  
  - New env created  
  - Work with condition, limitation and dynamic environment 

<a name="hw19"></a>
## Homework 19
<a name="hw191"></a>
##### Main task  
  - Create prometheus docker image  
  - Modify docker-compose.yml  
  - Setting up metrics collection  
  - Work with exporters  

  - Dockerhub link  
> https://hub.docker.com/u/alexotusdevops/

<a name="hw20"></a>
## Homework 20
<a name="hw201"></a>
##### Main task  
  - Separate docker-compose files  
  - Create grafana docker image  
  - Create dashboards  
  - Work with alertmanager  

  - Dockerhub link  
> https://hub.docker.com/u/alexotusdevops/

<a name="hw21"></a>
## Homework 21
<a name="hw211"></a>
##### Main task  
  - Configured EFK stack  
  - Create & configured filters and log parsing rules  
  - Add zipkin in docker-compose-logging  

<a name="hw22"></a>
## Homework 22
<a name="hw221"></a>
##### Main task  
  - Set up Kubernetes the hard way  

<a name="hw23"></a>
## Homework 23
<a name="hw231"></a>
##### Main task  
  - Run reddit app locally in Minikube  
  - Run reddit app in GCE  
  - App link: http://35.193.251.105:30090/  

<a name="hw24"></a>
## Homework 24
<a name="hw241"></a>
##### Main task  
  - Ingress Controller  
  - Ingress  
  - Secret  
  - TLS  
  - LoadBalancer Service  
  - Network Policies  
  - PersistentVolumes  
  - PersistentVolumeClaims  

<a name="hw25"></a>
## Homework 25
<a name="hw251"></a>
##### Main task  
  - Install prometheus, grafana, EFK on kubernetes cluster  


