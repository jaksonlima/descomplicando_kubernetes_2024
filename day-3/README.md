# kubectl commands

```
k get deployments.apps deploy-nginx -o yaml > deploy-temp.yaml

k create deployment --image nginx --replicas 3 deploy-nginx

k create deployment --image nginx --replicas 3 deploy-nginx --dry-run=client
```
