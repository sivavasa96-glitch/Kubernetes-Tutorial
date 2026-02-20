Important commands used:
========================
___
kubectl version: 
Shows kubectl client and Kubernetes server version.


kubectl get pods – Shows all running pods in the cluster.

kubectl get pods -n kube-system – Lists system pods in kube-system namespace.

kubectl get pods -l app=nginx – Shows pods with label app=nginx.

kubectl describe pod etcd-minikube -n kube-system – Shows detailed info about etcd-minikube pod.

kubectl describe pod – Shows detailed information about a specific pod.

kubectl run althaf-nginx --image=nginx – Creates and runs a pod using nginx image.

kubectl exec -it althaf-nginx -- /bin/bash – Opens terminal inside the pod.

kubectl exec -it -- /bin/sh – Opens shell inside running pod.

kubectl exec -it -- /bin/sh -c 'echo $WELCOME_MSG' – Displays ConfigMap value inside pod.

kubectl exec -it -- /bin/sh -c 'echo $ADMIN_PASSWORD' – Displays Secret value inside pod.

kubectl delete pod althaf-nginx – Deletes the specified pod.

kubectl delete pod – Deletes a specific pod.

kubectl create deployment althaf-nginx --image=nginx – Creates a deployment using nginx image.

kubectl delete deployment althaf-nginx – Deletes the deployment and its pods.

kubectl scale deployment althaf-nginx --replicas=5 – Scales deployment to run 5 pods.

kubectl apply -f nginx-configmap.yaml – Creates ConfigMap to store configuration values.

kubectl apply -f nginx-secret.yaml – Creates Secret to store sensitive data like passwords.

kubectl apply -f nginx-deployment.yaml – Creates Deployment and runs nginx pods using YAML file.

kubectl apply -f nginx-service.yaml – Creates Service to expose nginx pods.

kubectl get svc – Lists all services in the cluster.

kubectl get svc nginx-service – Shows details of nginx-service including port and IP.

kubectl rollout restart deployment nginx-deployment – Restarts deployment and recreates pods.

kubectl cluster-info – Displays Kubernetes cluster information.

minikube start – Starts local Kubernetes cluster.

minikube ip – Shows Minikube cluster IP address.

minikube service nginx-service --url – Shows URL to access nginx service in browser.

---