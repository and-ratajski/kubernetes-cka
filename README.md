# Self-managed Kubernetes Cluster auxiliary tools

Please mind that this tools were meant for and to be used on [bare metal kubernetes](https://ubuntu.com/blog/understanding-bare-metal-kubernetes) cluster!

- [_kubectl-api-proxy](./_kubectl-api-proxy/)
    Solution on how to connect to Kubernetes Cluster (that exposes an ingress) running on machine in a private network (allows HTTPS connectionion). Other way would be  using [Proxy Verb](https://kubernetes.io/docs/tasks/access-application-cluster/access-cluster-services/)

- [keycloak-single-db](./keycloak-single-db/)
    [Keycloak](https://www.keycloak.org/) kubernetes deployment prepared in a single data-base mode.

- [nginx-ingress](./nginx-ingress/)
    [NGINX Ingress Controller](https://kubernetes.github.io/ingress-nginx/) for bare metal kubernetes cluster and Kubernetes Ingress that uses it. It allows comminication with the cluster (_develop_ namespace) (other way would be via `kubectl proxy`)

- [nginx-ingress-dashboard](./nginx-ingress-dashboard/)
    An ingress to reach Kubernetes Dashboard (_kubernetes-dashboard_ namespace)

- [nginx-test](./nginx-test/)
    Test deployment of a simple nginx service to act as a default service and health checker for _develop_ namespace

- [traefik-ingress](./traefik-ingress/)
    Traefik run in ingress mode (under development)

## Possible issues

### DNS resolution

This issue occurs especially on Ubuntu-based VMS

https://stackoverflow.com/a/74549954/16775898
