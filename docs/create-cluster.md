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

![cluster-info](../assets/cluster-info.png)

### Start the dashboard

```bash
minikube dashboard
```

![dashboard](../assets/dashboard.png)

Other services and commands related to minikube can be found [here](https://minikube.sigs.k8s.io/docs/start/)