pod is running but you see 0/1 i.e. Not Ready
(port-forwarding works since it is a special case. Don't do port-forwarding for this case)

kubectl describe pod <pod-name>
kubectl get endpoints

NO Endpoints though the matchLabels match.
Only READY PODS become Service Endpoints
