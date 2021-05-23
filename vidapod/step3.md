Usually you don't need to create Pods directly, even singleton Pods. Instead, create them using workload resources such as Deployment or Job. 

Pods in general run a single container. The "one-container-per-Pod" model is the most common Kubernetes use case; in this case, you can think of a Pod as a wrapper around a single container; Kubernetes manages Pods rather than managing the containers directly.

In this command, you'll use the Deployment resource to launch a single container of nginx

`kubectl create deployment nginx --image=nginx`{{execute}}

Wait for the Deployment to become ready by checking

`kubectl get pods`{{execute}}