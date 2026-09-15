# NVIDIA Dynamo serving

Match the Dynamo/backend versions, topology, hardware, and Kubernetes access. Runtime bring-up and diagnosis use bundled scripts; recipe discovery needs the Dynamo `recipes/` tree. The assigned-deployment and AIPerf experiment workflows additionally require a Dynamo checkout with `agent-docs`, workload records, deployment ledgers, and run artifacts. Installing individual skills does not supply that external experiment context.

## Recipe selection and deployment

| Skill | Install source | Use when |
| --- | --- | --- |
| `find-serving-recipe` | `ai-dynamo/dynamo` | A model, hardware budget, and workload need a source-backed serving recipe dossier with provenance and confidence before baseline selection or a new optimization experiment. |
| `dynamo-recipe-runner` | `NVIDIA/skills` | An existing Dynamo Kubernetes recipe needs discovery, lightweight validation, minimal manifest patches, deployment, and endpoint smoke verification. |
| `deploy-dynamo-recipe` | `ai-dynamo/dynamo` | A Dynamo experiment has an assigned baseline or approved candidate DGD and needs deployment ledgers, readiness checks, and a smoke-test artifact without substituting or tuning the assigned configuration. |

Use `dynamo-recipe-runner` for ordinary catalog-based bring-up. Use `deploy-dynamo-recipe` when the experiment workflow owns an exact DGD and its identity. They represent different deployment workflows rather than two default steps for the same task.

## Routing, transport, and diagnosis

| Skill | Install source | Use when |
| --- | --- | --- |
| `dynamo-router-starter` | `ai-dynamo/dynamo` | Dynamo round-robin, KV-aware, least-loaded, or device-aware routing needs configuration and endpoint smoke checks. |
| `dynamo-interconnect-check` | `ai-dynamo/dynamo` | Disaggregated or multi-node Dynamo serving needs NIXL/UCX/NCCL environment, RDMA/NVLink capabilities, and transfer-test readiness checks before trusting performance results. |
| `troubleshoot-dynamo` | `ai-dynamo/dynamo` | Dynamo pods, model-cache jobs, PVCs, operator resources, workers, frontend/router, endpoints, or benchmark jobs need read-only evidence collection and failure classification. |

## Reproducible AIPerf experiments

| Skill | Install source | Use when |
| --- | --- | --- |
| `configure-aiperf-benchmark` | `ai-dynamo/dynamo` | A smoke-tested Dynamo candidate needs a frozen, question-driven workload, SLOs, load policy, versioned benchmark plan, and Kubernetes benchmark manifests. |
| `run-aiperf-benchmark` | `ai-dynamo/dynamo` | A configured Dynamo AIPerf Job needs bounded execution, monitoring, ownership-based failure handoffs, and unchanged raw artifact collection. |
| `analyze-aiperf-results` | `ai-dynamo/dynamo` | Completed AIPerf runs need evidence validity checks, normalized summaries, SLO/goodput analysis, and comparison with compatible prior measurements. |

The experiment chain is configuration → execution → evidence audit and analysis. Match the active workload and plan identities across those steps; Job completion alone does not establish valid evidence.

## Frontend performance

| Skill | Install source | Use when |
| --- | --- | --- |
| `dynamo-frontend-benchmark` | `ai-dynamo/dynamo` | Dynamo frontend, tokenizer, or KV-router changes need throughput/latency comparisons or CPU profiling against mock workers, with a built matching checkout and the source's isolation tooling available. |

For engine-specific server tuning or general endpoint benchmarks, open [model serving](serving.md). For GPU kernels, open [CUDA and GPU acceleration](../systems/cuda.md). For cluster delivery, open [Kubernetes and delivery](../infrastructure/kubernetes-delivery.md).
