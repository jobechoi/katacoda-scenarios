 To effectivley work with Pods, you need to at least have an understanding of how pods relate to the other Kubernetes components.

## Task

To start we need to launch a Kubernetes cluster.

Execute the command below to start the cluster components and download the Kubectl CLI.

`minikube start --wait=false`{{execute}}

The Kubectl CLI is a command line tool lets you control Kubernetes clusters.

Wait for the Node to become Ready by checking 

`kubectl get nodes`{{execute}}

