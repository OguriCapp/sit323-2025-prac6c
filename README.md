For this Task6.2C, I still used the same codes from 6.1P and I used Git Bash to check and forward ports. 
Firstly, I type to see my running application status:
kubectl get pods
kubectl get services

From this I got my service name and saw it uses port 80. Then I ran port forward command to transport it from 80 to 6262:

kubectl port-forward svc/sit323-61p-app-service 6262:80

This changed port from 80 to 6262. After testing, all math functions like add/subtract/power and etc worked fine at localhost:6262.
