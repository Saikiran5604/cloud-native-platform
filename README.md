# Cloud Native Platform

Building a production-grade Kubernetes platform on AWS — from Linux fundamentals to multi-cluster orchestration.

## What This Is

A hands-on journey through cloud-native infrastructure, starting from Linux primitives (processes, namespaces, cgroups) and building up to a fully operational Kubernetes platform with networking, storage, monitoring, and security.

## Learning Path

| Stage | Topic | What's Covered |
|-------|-------|----------------|
| 1 | **Linux Fundamentals** | Shell, process management, signals |
| 2 | **Processes & Isolation** | Process trees, PID namespaces, resource limits |
| 3 | **Namespaces** | Network, mount, user, and PID isolation — the building blocks of containers |
| 4 | **cgroups** | CPU, memory, and I/O resource control |
| 5 | **Containers** | Building containers from scratch, Docker, containerd |
| 6 | **Kubernetes** | Architecture, API server, etcd, kubelet, scheduler |
| 7 | **Networking** | CNI plugins, Service networking, DNS, Ingress |
| 8 | **Storage** | PVs, PVCs, CSI drivers, StatefulSets |
| 9 | **Monitoring** | Prometheus, Grafana, alerting |
| 10 | **Security** | RBAC, NetworkPolicies, Kyverno, Pod Security Standards |
| 11 | **CI/CD** | GitOps with Argo CD, image pipelines |

## Structure

```
docs/               ← Deep-dive notes on each topic
labs/               ← Hands-on exercises and experiments
├── day02-processes/
├── day03-namespaces/
└── day04-cgroups/
```

## Platform Stack

- **Orchestration:** Kubernetes (EKS)
- **Networking:** Istio service mesh, Calico CNI
- **Policy:** Kyverno for admission control
- **Monitoring:** Prometheus + Grafana
- **GitOps:** Argo CD
- **IaC:** Terraform

## Related Repos

- [register-app](https://github.com/Saikiran5604/register-app) — Full CI/CD pipeline deploying to this platform
- [gitops-register-app](https://github.com/Saikiran5604/gitops-register-app) — GitOps manifests synced via Argo CD
