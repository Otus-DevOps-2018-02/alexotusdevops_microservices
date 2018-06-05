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


