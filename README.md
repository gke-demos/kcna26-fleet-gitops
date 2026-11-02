# kcna26-fleet-gitops

Desired state for the KubeCon NA 2026 kube-agents demo fleet. Config Sync applies
`clusters/<cluster>/` to each cluster; the kube-agents Platform Agent proposes every change as a
pull request here and never writes to a cluster itself. A human merges.

| Cluster         | App                                                                                 |
| --------------- | ----------------------------------------------------------------------------------- |
| `boutique-prod` | [Online Boutique](https://github.com/GoogleCloudPlatform/microservices-demo) v0.10.7 |
| `bank-prod`     | [Bank of Anthos](https://github.com/GoogleCloudPlatform/bank-of-anthos) v0.6.11      |

This repository is a demo: it contains deliberately planted misconfigurations for the agent to
find. Do not copy it as a template. The demo's scripts and runbook are in
[`gke-demos/kcna26-kube-agents`](https://github.com/gke-demos/kcna26-kube-agents).
