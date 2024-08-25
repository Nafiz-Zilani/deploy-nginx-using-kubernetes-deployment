kubectl create -f deployment-definition.yaml
kubectl create deployment nginx-deployment --image=nginx:latest --replicas=6 --port=80
kubectl get deployments
kubectl delete deployment nginx-deployment

kubectl get pods


//Get Pods ID
kubectl get pod nginx-deployment-8bd988c94-7x55s -o jsonpath='{.status.podIP}'

Curl to pod
curl http://10.42.1.15:80
# deploy-nginx-using-kubernetes-deployment
