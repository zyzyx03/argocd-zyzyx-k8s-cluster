# Cluster Bootstrapping Using ArgoCD App of Apps Patter

Utilizing [App-of-Apps](https://argoproj.github.io/argo-cd/operator-manual/cluster-bootstrapping/) pattern to provision cluster applications.

## Structure

```txt
argocd-zyzyx-k8s-cluster
├── README.md
├── rke2-infra-apps         <-- Directory with child Apps
│   ├── cert-manager.yaml
│   ├── falco.yaml
│   ├── gatekeeper.yaml
│   ├── ingress-nginx.yaml
│   └── longhorn.yaml
└── root-rke2-infra         <-- Directory for Root ArgoCD application
    └── my-rke2-cluster.yaml
```

## Known Issues
