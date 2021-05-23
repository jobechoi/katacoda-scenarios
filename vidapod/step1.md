 To effectivley work with Pods, you need to at least have an understanding of how pods relate to the other Kubernetes components.

## Task

To start we need to launch a Kubernetes cluster.

Execute the command below to start the cluster components and download the Kubectl CLI.

`minikube start --wait=false`{{execute}}

The Kubectl CLI is a command line tool that lets you control Kubernetes clusters.

Kubernetes runs your workload by placing containers into Pods to run on Nodes. A node may be a virtual or physical machine, depending on the cluster. Typically you have several nodes in a cluster; in a learning or resource-limited environment, you might have only one node.

Wait for the Node to become Ready by checking 

`kubectl get nodes`{{execute}}