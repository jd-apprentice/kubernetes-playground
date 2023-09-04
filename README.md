# kubernetes-playground

## Requirements 🧰

- [Kubectl](https://kubernetes.io/docs/tasks/tools/#kubectl) 
- [Minikube](https://minikube.sigs.k8s.io/docs/start/)

## Create a cluster

![Diagram](https://d33wubrfki0l68.cloudfront.net/283cc20bb49089cb2ca54d51b4ac27720c1a7902/34424/docs/tutorials/kubernetes-basics/public/images/module_01_cluster.svg)

Important points

- The Control Plane is responsible for managing the cluster.
- A node is a VM or a physical computer that serves as a worker machine in a Kubernetes cluster.
- Node-level components, such as the kubelet, communicate with the control plane using the Kubernetes API

### Start minikube

```bash
minikube start
```

### Check cluster status

```bash
kubectl cluster-info
```

![cluster-info](./assets/cluster-info.png)

### Start the dashboard

```bash
minikube dashboard
```

![dashboard](./assets/dashboard.png)

Other services and commands related to minikube can be found [here](https://minikube.sigs.k8s.io/docs/start/)

## Using kubectl to create a Deployment

### Objectives

- Learn about application Deployments.
- Deploy your first app on Kubernetes with kubectl.

![diagram](./assets/diagram-deployment.png)

- You can create deployments using `kubectl` which communicates with kubernetes API.

#### kubectl basics

The common format of a kubectl command is: `kubectl action resource`

To deploy an app we can use the following command:

```bash
kubectl create deployment kubernetes-bootcamp --image=gcr.io/google-samples/kubernetes-bootcamp:v1
```

To list the deployments:

```bash
kubectl get deployments
```

![deployments](./assets/deployments.png)