In this scenario, you did the following

** Start the cluster components and download the Kubectl CLI.

`minikube start --wait=false`

** Check Nodes 

`kubectl get nodes`

** Deployment resource to launch a single container of nginx

`kubectl create deployment nginx --image=nginx`

** Check Deployment

`kubectl get pods`

** Create a Horizontal Pod Autoscaler for Deployment

`kubectl autoscale deployment nginx --cpu-percent=50 --min=1 --max=10`

** Check status of autoscaler

`kubectl get hpa`