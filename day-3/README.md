# kubectl commands

```
k get deployments.apps deploy-nginx -o yaml > deploy-temp.yaml

k create deployment --image nginx --replicas 3 deploy-nginx

k create deployment --image nginx --replicas 3 deploy-nginx --dry-run=client

k create namespace deploy-namespace --dry-run=client -o yaml > namespace-deploy.yaml

k get all -n deploy-namespace

k exec -it -n deploy-namespace pods/deploy-namespace-nginx-78b9f6fff8-25xrj -- nginx -v

k exec -it -n deploy-namespace pods/deploy-namespace-nginx-78b9f6fff8-25xrj -c container-nginx -- bash

k rollout status deployment -n deploy-namespace deploy-namespace-nginx

k rollout undo deployment deploy-nginx

k rollout history deployment deploy-nginx

k rollout history deployment deploy-nginx --revision 2

k rollout undo  deployment deploy-nginx --to-revision 1

k rollout pause deployment deploy-nginx

k rollout resume deployment deploy-nginx

k scale deployment deploy-nginx --replicas 1
```
