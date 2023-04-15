# NGINX Ingress Controller

https://kubernetes.github.io/ingress-nginx/deploy/#bare-metal-clusters

## Grant kubectl access to priviliged ports

https://stackoverflow.com/a/55023272/16775898

```shell
sudo setcap CAP_NET_BIND_SERVICE=+eip /usr/local/bin/kubectl
```

## Enable port forwarding to the ingress controller

```shell
kubectl port-forward --address 0.0.0.0 --namespace=ingress-nginx service/ingress-nginx-controller 80 443
```

## Mind ingress limitiations

https://stackoverflow.com/a/63167986/16775898

## Use annotations

https://kubernetes.github.io/ingress-nginx/user-guide/nginx-configuration/annotations/#external-authentication
