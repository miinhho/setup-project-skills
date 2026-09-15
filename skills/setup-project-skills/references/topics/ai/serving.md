# Model serving

Match the serving engine, backend, installed versions, hardware, and workload before proposing a skill. Check example commands against the installed CLI and current runtime docs, especially build flags, image tags, quantization formats, and performance assumptions.

For provider-specific work, open only the matching map:

| Field | Open when | Map |
| --- | --- | --- |
| Managed and cloud serving | SageMaker, Google Cloud Agent Platform, Databricks, Modal, or GKE hosts the model endpoint. | [Managed and cloud serving](managed-serving.md) |
| Dynamo | Distributed serving, KV-aware routing, disaggregated transport, or Dynamo performance experiments recur. | [Dynamo](dynamo.md) |
| Jetson | Jetson runtime selection, memory tuning, benchmarking, or speculative decoding recur. | [Jetson serving](jetson-serving.md) |

## Local model serving

| Skill | Install source | Use when |
| --- | --- | --- |
| `huggingface-local-models` | `huggingface/skills` | Local GGUF model selection, quantization, conversion, and llama.cpp serving recur. |
| `llama-cpp` | `orchestra-research/ai-research-skills` | llama.cpp layer offload, context sizing, grammar-constrained generation, or server tuning recur beyond model selection; verify build examples against the installed version. |

## vLLM deployment and runtime tuning

| Skill | Install source | Use when |
| --- | --- | --- |
| `vllm-deploy-simple` | `vllm-project/vllm-skills` | A local vLLM install, OpenAI-compatible server startup, and inference smoke test recur. |
| `vllm-deploy-docker` | `vllm-project/vllm-skills` | vLLM Docker images, GPU access, container launch flags, or containerized endpoint verification recur. |
| `vllm-deploy-k8s` | `vllm-project/vllm-skills` | vLLM Kubernetes Deployments, Services, GPU resources, or health probes recur. |
| `serving-llms-vllm` | `orchestra-research/ai-research-skills` | vLLM batch inference, tensor parallelism, quantized serving, or runtime performance tuning recur beyond server bring-up. |

## Other serving engines and diagnosis

| Skill | Install source | Use when |
| --- | --- | --- |
| `sglang` | `orchestra-research/ai-research-skills` | SGLang structured outputs, prefix caching, tool calling, or serving configuration recur. |
| `trtllm-serve-config-guide` | `NVIDIA/TensorRT-LLM` | A checked-out TensorRT-LLM config database and deployment docs can ground single-node aggregate PyTorch serving YAML for an explicit latency or throughput objective. |
| `tensorrt-llm` | `orchestra-research/ai-research-skills` | TensorRT-LLM batching, quantized serving, multi-GPU setup, or runtime integration recur beyond the official guide's single-node config scope; match the actual backend and version. |
| `deployment` | `NVIDIA/model-optimizer` | A Hugging Face-format or ModelOpt checkpoint needs vLLM, SGLang, or TRT-LLM serving with quantization detection, server lifecycle management, health checks, and API verification. |

## SGLang diagnosis and runtime profiling

| Skill | Install source | Use when |
| --- | --- | --- |
| `sglang-prod-incident-triage` | `sgl-project/sglang` | SGLang serving health, queue growth, latency, crashes, or output regressions need evidence collection and request replay before deeper debugging. |
| `debug-cuda-crash` | `sgl-project/sglang` | A reproduced SGLang CUDA crash needs kernel API logging, input-tensor dumps, or compute-sanitizer/cuda-gdb diagnosis in a matching runtime or checkout. |
| `debug-distributed-hang` | `sgl-project/sglang` | A reproduced SGLang TP/PP/DP/EP stall needs per-rank state comparison, collective-hang localization, and verification that ranks follow the same execution path. |
| `llm-torch-profiler-analysis` | `sgl-project/sglang` | SGLang, vLLM, TensorRT-LLM, or TokenSpeed torch-profiler traces need kernel, overlap, or fusion analysis; check the source's backend capability matrix before requesting live capture. |

The TensorRT-LLM config guide requires access to that repository's checked-in configs and docs; installing its skill alone does not supply them. SGLang replay and deeper CUDA, distributed-hang, or profiler diagnosis may also require a matching SGLang checkout and the focused skills named by its triage workflow.

## BentoML service creation and deployment

| Skill | Install source | Use when |
| --- | --- | --- |
| `bentoml-create-bento` | `bentoml/BentoML` | Models, scripts, notebooks, or existing APIs become typed BentoML services with tested outputs, streaming, adaptive batching, or service dependencies. |
| `bentoml-containerize` | `bentoml/BentoML` | A BentoML project needs a built Bento, an OCI image, a real inference smoke test, and registry push. |
| `bentoml-k8s-deploy` | `bentoml/BentoML` | A containerized BentoML service needs plain Kubernetes deployment, service-specific sizing, dependency wiring, rollout verification, or deployment diagnosis. |
| `bentoml-ec2-deploy` | `bentoml/BentoML` | A containerized BentoML service deploys directly to existing or newly provisioned EC2 hosts over SSH and Docker, with per-host inference verification. |
| `bentoml-deploy-scriptgen` | `bentoml/BentoML` | BentoML Kubernetes or EC2 deployments need a committable script bundle and configuration that run from a terminal or CI without an agent. |

Keep the selected skills' bundled references and templates. `bentoml-k8s-deploy` uses the sibling `bentoml-deploy-scriptgen` templates for rendering and validation; propose both when that deployment workflow is needed. Add `bentoml-containerize` when image building is part of the work. Interactive deployment and repeatable CI deployment are separate responsibilities.

## Serving benchmarks

| Skill | Install source | Use when |
| --- | --- | --- |
| `vllm-bench-serve` | `vllm-project/vllm-skills` | vLLM or another OpenAI-compatible endpoint needs TTFT, TPOT, throughput, or goodput benchmarks. |
| `vllm-bench-random-synthetic` | `vllm-project/vllm-skills` | A serving endpoint needs a quick synthetic-workload baseline without downloading an external dataset. |
| `vllm-prefix-cache-bench` | `vllm-project/vllm-skills` | Repeated-prefix workloads need measured automatic prefix-cache effectiveness. |
| `hybrid-benchmarking` | `LMCache/LMCache` | A hybrid-attention model needs controlled comparisons of the vLLM allocator, GPU prefix caching, and LMCache; the matching LMCache checkout, recipes, and GPU capacity are available. |

For model training, evaluation, or embedded inference, open [machine learning](ml.md). For CUDA kernel development or profiling, open [CUDA and GPU acceleration](../systems/cuda.md). For deployment infrastructure, open [Kubernetes and delivery](../infrastructure/kubernetes-delivery.md) or [GKE](../infrastructure/gke.md).
