kubectl apply -f configmap.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

kubectl port-forward service/config-demo-service 8080:80

Edit configmap with Version 2 and
kubectl apply -f configmap.yaml

Refresh browser

kubectl rollout restart deployment config-demo
