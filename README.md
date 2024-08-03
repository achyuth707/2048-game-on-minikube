# 2048-game-on-minikube

Pre-requisites (Download from official sites)

•	Install Minikube on windows

•	Install Docker Desktop (Install required components for WSL 2)

•	Install kubectl 

Start Minikube with docker as driver

•	Start the docker engine (Open Docker Desktop and the engine will be started automatically)

•	minikube start –driver=docker

•	minikube status

*DOCKER Commands*

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

*Kubernetes Commands*

kubectl get nodes 				          -->  # Display all node information

kubectl get nodes -o wide   	          -->  # Show more information about all nodes

kubectl get pods 				          -->  # Display all container group information

kubectl get pods -o wide    	          -->  # Show more information about all pods

kubectl get ns					          -->  # Display all namespace information

kubectl get ns -o yaml      	          -->  # Show yaml information about all namespaces

kubectl get ns -o wide      	          -->  # Show more information about all namespaces

kubectl get deploy				          -->  # Display all deployments information

kubectl describe deploy 		          -->  # Describe deployments information

kubectl get deploy -o wide  	          -->  # Show more information about all deployments

kubectl get deploy -o yaml  	          -->  # Show yaml information about all deployments

kubectl apply -f deployment.yaml          -->  # To start the deployment

kubectl delete -f deployment.yaml         -->  # To delete the deployment

kubectl get all -n <namespace>		      -->  # To get all the resources from specific namespace

kubectl get svc						      -->  # Display all services information

kubectl get ingress					      -->  # Display all ingress information

kubectl logs -n <namespace> <pod-name>	  -->  # To fetch the logs from pod-name

*Minikube Commands*

minikube start 								   --> # To start minikube cluster

minikube start --driver=docker				   --> # To start minikube with specific driver

minikube delete								   --> # To delete minikube

minikube addons enable ingress				   --> # To enable ingress controller using minikube addons

minikube ip									   --> # To fetch minikube ip

minikube tunnel								   --> # To create a network tunnel that allows services with type LoadBalancer to be accessible on your local network

minikube addons disable ingress 			   --> # To disable ingress controller using minikube addons

minikube update-check 						   --> # To check if there is a newer version of minikube available

minikube status								   --> # To check minikube status

minikube dashboard 							   --> # It will open kubernetes cluster in your default browser

minikube dashboard --url					   --> # It will give URL for kubernetes cluster

minikube service <service name> --namespace=<namespace> --> # To retrieve the URL where the service can be accessed

minikube service ingress-nginx-controller --namespace=ingress-nginx --url --> # To retrieve the URL where the service can be accessed
