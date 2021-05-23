Now that the deployment is running, we will create a Horizontal Pod Autoscaler for it. To create it, we will use kubectl autoscale command, which looks like this:

`kubectl autoscale deployment nginx --cpu-percent=50 --min=1 --max=10`{{execute}}

This defines a Horizontal Ppod Autoscaler that maintains between 1 and 10 replicas of the Pods controlled by nginx deployment we created in Step 3. 

Broadly speaking, the horizontal autoscaler will increase and decrease the number of replicas (via the deployment) so as to maintain an average CPU utilization across all Pods of 50% (since each pod requests 500 milli-cores by kubectl run, this means average CPU usage of 250 milli-cores). 

We may check the current status of autoscaler by running:

`kubectl get hpa`{{execute}}