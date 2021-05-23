Kubernetes runs your workload by placing containers into Pods to run on Nodes. A node may be a virtual or physical machine, depending on the cluster. 

Typically you have several nodes in a cluster; in a learning or resource-limited environment, you might have only one node.

Wait for the Node to become Ready by checking 

`kubectl get nodes`{{execute}}