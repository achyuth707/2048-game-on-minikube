# 2048-game-on-minikube

Pre-requisites (Download from official sites)

•	Install Minikube on windows

•	Install Docker Desktop (Install required components for WSL 2)

•	Install kubectl 

Start Minikube with docker as driver

•	Start the docker engine (Open Docker Desktop and the engine will be started automatically)

•	minikube start –driver=docker

•	minikube status

DOCKER Commands 
docker login												 --> Login to your docker hub

docker pull achyuth707/webpage-cmd 							 --> To pull the image from docker hub

docker push achyuth707/webpage-cmd 							 --> To push the image from docker hub

docker ps										             --> List running containers

docker ps -a									             --> List all containers

docker ps -s									             --> List running containers (with CPU / memory)

docker images									             --> List all images

docker exec -it <container id> bash							 --> Connecting to container

docker logs <container id>	    				             --> Shows container's console log

docker stop <container id>	    				             --> Stop a container

docker restart <container id>					             --> Restart a container

docker rm <container id>	    				             --> Remove a container

docker port <container id>	    				             --> Shows container's port mapping

docker top <container id>	    				             --> List processes

docker kill <container id>	    				             --> Kill a container

docker build -t achyuth707/webpage-cmd .					 --> To build an image using docker file

docker run -d -p 8080:80 achyuth707/webpage-cmd              --> To start a container

docker start <container id>						             --> To Start

docker stop <container id>						             --> To Stop

docker restart <container id>					             --> To Restart

docker inspect <container id>	                             --> Inspecting Containers

docker events <container id>	                             --> Containers Events

docker port <container id>	                                 --> Public Ports

docker top <container id>	                                 --> Running Processes

docker rename achyuth707/webpage-cmd achyuth707/webpage-achu --> Rename

docker images 												 --> Listing images

docker rmi <Image ID>										 --> Removing an image

docker history												 --> history of an image
