--> Start the docker engine (Open Docker desktop, It will start the docker engine automatically)

--> minikube start --driver=docker (Start minikube with docker as primary docker)

--> verify whether all the pre-requisites are installed or not

    kubectl version && minikube version && docker version

--> clone my git repo using - git clone https://github.com/achyuth707/2048-game-on-minikube.git

--> Add Ingress controller using minikube addons - minikube addons enable ingress

--> Run below commands to create deployment, service and ingress

    kubectl apply -f 2048-deployment.yaml
    
    kubectl apply -f 2048-service.yaml
    
    kubectl apply -f 2048-ingress.yaml

--> verify resources created or not from minikube dashboard

    minikube dashboard 							   --> # It will open kubernetes cluster in your default browser
    
    minikube dashboard --url					   --> # It will give URL for kubernetes cluster

--> verify the same using kubectl commands

    kubectl get nodes 				          -->  # Display all node information
    
    kubectl get nodes -o wide   	          -->  # Show more information about all nodes
    
    kubectl get pods 				          -->  # Display all container group information
    
    kubectl get pods -o wide    	          -->  # Show more information about all pods
    
    kubectl get ns					          -->  # Display all namespace information
    
    kubectl get ns -o wide      	          -->  # Show more information about all namespaces
    
    kubectl get deploy				          -->  # Display all deployments information
    
    kubectl get deploy -o wide  	          -->  # Show more information about all deployments
    
    kubectl get svc						      -->  # Display all services information
    
    kubectl get svc	-o wide					  -->  # Show more information about all services
    
    kubectl get ingress					      -->  # Display all ingress information
    
    kubectl get ingress	-o wide				  -->  # Show more information about all ingress
    
    kubectl logs -n <namespace> <pod-name>	  -->  # To fetch the logs from pod-name


--> Fetch the minikube ip and add it to the hosts file under c/windows/system32/drivers/etc/

    <minikube ip> <loadbalancer>

--> Open minikube network tunnel that allows services with type LoadBalancer to be accessible on your local network

    minikube tunnel

--> Access the LoadBalancer using local browser


##### Happy Playing 2048 #####
    
