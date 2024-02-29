# Pod

```
kubectl get pod -o wide

k get pod nginx -o yaml

k get pods -L run

k get pods -A

k delete pod nginx

k get pod jakson-lima -o yaml > pod-created.yam

k run jakson --image nginx --port 80 --dry-run=client -o yaml

k exec pods/nginx-1 -it -- bash

k exec pods/nginx -- cat /usr/share/nginx/html/index.html
```

# Stress Pod

```
k exec pods/limitado -it -- bash

apt-get update && apt-get install -y stress

stress --cpu 1 --vm 1 --vm-bytes 110M
```
