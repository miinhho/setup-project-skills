# Kubernetes and delivery

## Workloads and diagnosis

| Skill | Install source | Use when |
| --- | --- | --- |
| `kubernetes-patterns` | `affaan-m/ECC` | Built-in workload manifests, probe semantics, ServiceAccount access, HPA, or disruption budgets recur. |
| `k8s-debug` | `akin-ozer/cc-devops-skills` | kubectl-based pod, DNS, storage, node-pressure, or rollout diagnosis needs evidence gathering and fix verification; kubectl and cluster read access are available. |

## Helm

| Skill | Install source | Use when |
| --- | --- | --- |
| `helm-charts` | `bagelhole/devops-security-agent-skills` | Helm 3 chart authoring, helpers, conditional templates, hooks, library charts, or OCI packaging recur. |
| `helm-validator` | `akin-ozer/cc-devops-skills` | Existing charts need Helm lint/render checks, rendered YAML/schema validation, CRD checks, and a validation report; cluster dry-run is optional. |

## GitOps

| Skill | Install source | Use when |
| --- | --- | --- |
| `argocd-gitops` | `bagelhole/devops-security-agent-skills` | Argo CD Applications, AppProjects, ApplicationSets, sync waves/hooks, notifications, or drift configuration recur. |
| `gitops-knowledge` | `fluxcd/agent-skills` | A Flux Operator project needs Flux CRD design or schema-checked manifests and has adopted the source's Operator lifecycle and RetryOnFailure policy. |
| `gitops-repo-audit` | `fluxcd/agent-skills` | A Flux Operator GitOps repository needs local manifest/overlay validation, deprecated-API checks, tenancy/secrets review, and a prioritized report; flux, flux-schema, and kustomize or kubectl are available. Confirm the source's Operator and retry-policy assumptions fit the project. |
| `gitops-cluster-debug` | `fluxcd/agent-skills` | A live Flux Operator installation needs source-to-applier dependency tracing, controller-log analysis, or reconciliation diagnosis; flux-operator-mcp is connected. |

## Istio and release practices

| Skill | Install source | Use when |
| --- | --- | --- |
| `istio-traffic-management` | `wshobson/agents` | An Istio project uses VirtualService/DestinationRule routing, weighted canaries, connection pools, bounded retries, or traffic mirroring. Check examples against the installed Istio API version. |
| `deployment-patterns` | `affaan-m/ECC` | Application release health checks, progressive delivery, rollback, or deployment verification recur. |

## Controller and CRD development

| Skill | Install source | Use when |
| --- | --- | --- |
| `k8s-api-conventions` | [Kubernetes SIG API conventions][k8s-api-conventions] | The repository develops Kubernetes controllers or CRDs and needs spec/status ownership, conditions, zero-versus-unset fields, bounded status/metrics, or API compatibility review. |

The Kubernetes SIG row covers controller/API development. Flux rows are maintained by the Flux project for Flux workflows; they are not general Kubernetes administration skills. For provider-specific official skills, open [GKE](gke.md) or the AWS EKS and Azure AKS rows in [cloud platforms](cloud-platforms.md). For artifact signing and supply-chain gates, open [security](security.md).

[k8s-api-conventions]: https://github.com/kubernetes-sigs/agent-sandbox/tree/main/.agents/skills/k8s-api-conventions
