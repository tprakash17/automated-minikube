An automated setup for local kubernetes development environment - Minikube
![](https://github.com/tprakash17/automated-minikube/blob/master/automated.jpg)

## Description
Kubernetes (K8s) is an open-source system for automating deployment, scaling, and management of containerized applications. If you and your team uses kubernetes cluster in production. How do you streamline your local developement setup with kubernetes. This project is about - setup an automated local k8s cluster. 

Objective is to provide similar k8s development environment to all the developers in the team. 
Few more points -

* Lower the setup time for the local k8s cluster.
* Production Parity.
* Consistent across all developers workstation.

## setup instructions ##

#### Install vagrant ####

```
$ sudo apt-get install vagrant
```

#### Clone this repository ####

```
$ git clone git@bitbucket.org:mediaiq/automated-minikube.git
$ cd automated-minikube
```

#### Run vagrant ####

```
$ vagrant up
```

#### SSH into vagrant box ####

```
$ vagrant ssh
```

#### Start minikube ####

```
$ sudo -E /usr/local/bin/minikube start --vm-driver=none
```

#### Verify and have a Happy Kubeing ####

```
$ kubectl get no
NAME       STATUS    ROLES     AGE       VERSION
minikube   Ready     master    1m        v1.13.2
```
