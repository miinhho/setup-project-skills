# Google Kubernetes Engine

These skills are maintained by Google in `google/skills` and apply to GKE. Match the cluster mode, installed versions, available CLI/MCP tools, and the project's chosen provisioning policy before proposing a row.

## Foundation and readiness

| Skill | Install source | Use when |
| --- | --- | --- |
| `gke-basics` | `google/skills` | GKE provisioning, credentials, onboarding, or workload deployment needs foundational guidance. |
| `gke-productionize` | `google/skills` | GKE production readiness needs a combined reliability, security, observability, backup, and cost assessment. |

## Networking

| Skill | Install source | Use when |
| --- | --- | --- |
| `gke-networking` | `google/skills` | GKE private endpoints, VPC-native address planning, DNS, Dataplane V2, or node egress recur; the project's provisioning policy fits the source's private-cluster assumptions. |
| `gke-service-networking` | `google/skills` | GKE Gateway API/HTTPRoute, GCE Ingress, NEG-backed load balancing, Cloud Armor, Certificate Manager, or Private Service Connect recur. |

## Diagnosis

| Skill | Install source | Use when |
| --- | --- | --- |
| `gke-workload-troubleshooting` | `google/skills` | GKE pods hit CrashLoopBackOff, OOMKilled, ImagePullBackOff, or Pending states. |
| `gke-node-notready` | `google/skills` | GKE node-health failures need read-only condition/event/log analysis that distinguishes runtime, resource, CNI, and admission-webhook problems. |
| `gke-workload-identity` | `google/skills` | GKE workload authentication fails and needs diagnosis across direct IAM principal binding, GSA impersonation, node-pool metadata mode, and metadata-server health. |

## Inference

| Skill | Install source | Use when |
| --- | --- | --- |
| `gke-inference` | `google/skills` | GKE Autopilot GPU/TPU model servers need Inference Quickstart profiles, optimized manifests, accelerator selection, or inference autoscaling; the source's cluster and CLI prerequisites fit. |

## Backup and recovery

| Skill | Install source | Use when |
| --- | --- | --- |
| `gke-backup-dr` | `google/skills` | Backup for GKE needs explicit volume/Secret inclusion, backup/restore plans, CMEK, conflict-policy handling, and restore verification. |

For generic workloads, Helm, Argo CD, Flux, or controller APIs, open [Kubernetes and delivery](kubernetes-delivery.md). For other cloud products, open [cloud platforms](cloud-platforms.md).

For managed model endpoints or other serving providers, open [managed and cloud serving](../ai/managed-serving.md).
