## Using kubectl to create a Deployment

### Objectives

- Learn about application Deployments.
- Deploy your first app on Kubernetes with kubectl.

![diagram](../assets/diagram-deployment.png)

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

![deployments](../assets/deployments.png)