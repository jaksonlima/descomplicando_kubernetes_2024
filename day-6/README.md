# kubectl commands

```
k get storageclass
k get storageclasses.storage.k8s.io

k get pv
k get persistentvolume
```

## Configuração nfs

```
sudo apt-get install -y nfs-kernel-server nfs-common

sudo vim /etc/exports

/mnt/nfs  *(rw,sync,no_root_squash,no_subtree_check)

mkdir /mnt/nfs && sudo chmod -R 777 nfs/

sudo exportfs -ar

showmount -e
```

## IP maquina

```
ip a | grep eth0
```
