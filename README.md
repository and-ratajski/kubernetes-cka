# Self-managed Kubernetes Cluster auxiliary tools

Please mind that this tools where meant for and used on [bare metal kubernetes](https://ubuntu.com/blog/understanding-bare-metal-kubernetes) cluster!

- [_kubectl-api-proxy](./_kubectl-api-proxy/)
    Solution on how to connect to Kubernetes Cluster (using [Proxy Verb](https://kubernetes.io/docs/tasks/access-application-cluster/access-cluster-services/)) running on machine in a private network when HTTPS connection is required.

- [keycloak-single-db](./keycloak-single-db/)
    [Keycloak](https://www.keycloak.org/) kubernetes deployment prepared in a single data-base mode.

- [nginx-ingress](./nginx-ingress/)
    [NGINX Ingress Controller](https://kubernetes.github.io/ingress-nginx/) for bare metal kubernetes cluster. It allows comminication with the cluster (other way is via `kubectl proxy`)

- [nginx-test](./nginx-test/)
    Test deployment of a simple nginx service to validate cluster config and if it's reachable from outside.

- [traefik-ingress](./traefik-ingress/)
    Traefik run in ingress mode (under development)
