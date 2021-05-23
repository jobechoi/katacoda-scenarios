In this scenario, you learned how to do the following

`minikube start --wait=false`
** Start the cluster components and download the Kubectl CLI.

`kubectl get nodes`
** Check Nodes 

`kubectl create deployment nginx --image=nginx`
** Deployment resource to launch a single container of nginx

`kubectl get pods`
** Check Deployment

`kubectl autoscale deployment nginx --cpu-percent=50 --min=1 --max=10`
** Create a Horizontal Pod Autoscaler for Deployment

`kubectl get hpa`
** Check status of autoscaler

