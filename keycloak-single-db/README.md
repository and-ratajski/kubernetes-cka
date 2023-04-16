# Keycloak full k8s deployment in a single-db mode

## Configuration

Configuration is done by [ConfigMaps and Secrets](2-configmaps-n-secrets.yaml). By default it expects to be hosted under https://accounts.localhost

## Persistent Storage

It uses [Local](https://kubernetes.io/docs/concepts/storage/storage-classes/#local) StorageClass provisioner so few reuirements have to be met before using it:

1. Label all the nodes that can create (and host) PesistentVolume with **effiware.com/allow-creating-pv=true** like so:

```shell
kubectl label nodes worker-node01 worker-node02 effiware.com/allow-creating-pv=true
```

2. On those nodes create directory where PV will be mounted

```shell
sudo mkdir -p /mnt/kubernetes/persistent_volumes/keycloak
```
