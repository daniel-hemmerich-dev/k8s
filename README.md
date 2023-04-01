# Kubernetes
Kubernetes was developed by Google and is a platform for managing containerised workloads and services in a declarative way.

## Prerequisites
You need to install the following components to run these examples on your local machine.

### kubectl
This is the Kubernetes command line tool for running commands on the Kubernetes cluster.
- Linux: https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/ 
- MacOs: https://kubernetes.io/docs/tasks/tools/install-kubectl-macos/
- Windows: https://kubernetes.io/docs/tasks/tools/install-kubectl-windows/ 

### minikube
This is a tool for running Kubernetes locally. https://minikube.sigs.k8s.io/docs/start/

## Commands
### Start minikube
```shell
minikube start
```

### Show the minikube dashboard
```shell
minikube dashboard
```

### Start a service with minkube
```shell
minikube service <service-name>
```

### List all minikube addons
```shell
minikube addons list
```

### Enable an addon of minikube
```shell
minikube addons enable <addon-name>
```

### Disable an addon of minikube
```shell
minikube addons disable <addon-name>
```

### Stop minikube
```shell
minikube stop
```

### Delete the minikube virtual machine
```shell
minikube delete
```

### Get deployments
```shell
kubectl get deployments
```

### Get pods
```shell
kubectl get pods
```

### Get services
```shell
kubectl get services
```

### Get events
```shell
kubectl get events
```

### Get multiple ressources
```shell
kubectl get pod/<pod-name> configmap/<configmap-name>
```

### Describe a ressource
```shell
kubectl describe configmap/<configmap-name>
```

### View the config
```shell
kubectl config view
```

### Create a deployment
```shell
kubectl create deployment hello-node --image=registry.k8s.io/e2e-test-images/agnhost:2.39 -- /agnhost netexec --http-port=8080
```

### Apply a ressource config
```shell
kubectl apply -f <file-path>
```

### Delete ressources
```shell
kubectl delete <service|deployment|...> <service-name>
```