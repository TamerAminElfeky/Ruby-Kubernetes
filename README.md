# Ruby-Kubernetes
Dockerize ruby and rails app , publish and scale with K8s

# Lab Environment

* Ubuntu 16.10
* Docker version 18.01.0-ce
* Docker-compose 1.16.1
* [Minikube](https://kubernetes.io/docs/tasks/tools/install-minikube/) v0.25.0
   * Kubernetes 1.8.0
   * kubelet 1.8.0
   * docker 17.09.0-ce
* GNU Make 
* vm-driver KVM 2.5.0


# Repo Branches
* Docker-compose
* Kubernetes: Envvars
* Kubernetes: ConfigMaps

# Docker-compose 
To build,initialize postgres and run the docker-compose stack , run the following command:
```
make dcompose-deploy
```

To clean the docker-compose containers and volumes , run the following command:

```
make dcompose-clean
```

# Kubernetes-Cluster

To initialize the project pods on kubernetes , run the following command:

```
make deploy
```

To clean the environment and delete all resource , run the following command:
```
make clean
```
