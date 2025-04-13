This is a simple Kubernetes deployment of a containerized web application which supports mathematical operations, including add, subtract, power and etc. This app is the same as Task 5.1P, but now deployed on a Kubernetes cluster.

For this task, I created two Kubernetes configuration files: deployment.yaml and service.yaml to define and set up the service about this app.

This deployment uses the Docker image oguricapp/sit323-61p-app and is exposed on port 80.

To deploy and use this application: You should firstly clone this repository and open git bash then type：

kubectl apply -f deployment.yaml kubectl apply -f service.yaml kubectl get services

Finally you could open localhost:80/... to use those functions.
