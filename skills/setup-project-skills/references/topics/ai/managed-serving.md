# Managed and cloud model serving

Match the actual provider, endpoint API, deployment pathway, and project's operating requirements. Propose the workflow steps the project needs together with their required sibling skills; account setup alone does not justify adding every provider skill.

## Amazon SageMaker

| Skill | Install source | Use when |
| --- | --- | --- |
| `hf-cloud-sagemaker-deployment-planner` | `huggingface/skills` | A Hugging Face or local model needs a SageMaker serving pathway chosen from model type, traffic shape, latency tolerance, hardware, and cost requirements. |
| `hf-cloud-aws-context-discovery` | `huggingface/skills` | The SageMaker workflow must resolve the actual AWS profile, region, account, and caller identity before using AWS APIs. |
| `hf-cloud-python-env-setup` | `huggingface/skills` | SageMaker deployment scripts need an isolated Python environment with compatible Python and current boto3. |
| `hf-cloud-sagemaker-iam-preflight` | `huggingface/skills` | SageMaker deployment needs a usable execution role or diagnosis of IAM preflight failures. |
| `hf-cloud-serving-image-selection` | `huggingface/skills` | A SageMaker deployment needs a compatible current serving image and region-specific URI for LLM, embedding, reranker, or other model inference. |
| `hf-cloud-sagemaker-production-defaults` | `huggingface/skills` | SageMaker real-time, inference-component scale-to-zero, or async endpoints need deployment scripts, autoscaling, CloudWatch alarms, inference verification, and teardown. |
| `aws-ai-ml` | `aws/agent-toolkit-for-aws` | The project needs SageMaker model selection, customization-to-deployment lifecycle orchestration, or endpoint diagnostics rather than only a focused Hugging Face serving workflow. |
| `sdk-getting-started` | `awslabs/agent-plugins` | The AWS Labs Serverless Model Customization deployment pathway needs its SageMaker Python SDK version, AWS region, and execution-role preflight. |
| `model-deployment` | `awslabs/agent-plugins` | Nova or OSS models LoRA-tuned through SageMaker Serverless Model Customization need the supported SageMaker or Bedrock deployment pathway. |

The Hugging Face planner hands off to AWS-context and Python-environment setup, IAM preflight, image selection, and production deployment. Keep the required sibling skills and their bundled scripts available for that pathway. `aws-ai-ml` is a broader lifecycle alternative. The AWS Labs `model-deployment` skill is specific to Serverless Model Customization LoRA outputs and requires `sdk-getting-started` when SDK preflight is missing, plus AWS MCP tools; it is not a generic base-model deployment skill.

## Google Cloud Agent Platform

| Skill | Install source | Use when |
| --- | --- | --- |
| `agent-platform-deploy` | `google/skills` | Agent Platform Model Garden models or custom weights need active endpoint deployment, operation-status checks, or deployment cleanup. |
| `agent-platform-endpoint-management` | `google/skills` | Agent Platform logical serving endpoints need creation, inventory, updates, traffic splitting, or permission/quota diagnosis. |

These skills cover the source's Agent Platform endpoint APIs. Check the product and API match before proposing them for a public Vertex AI project. Deployment and endpoint-resource management have distinct scopes.

## Google Kubernetes Engine

For GPU/TPU model servers on GKE, open [GKE inference](../infrastructure/gke.md#inference). For generic Kubernetes workloads, open [Kubernetes and delivery](../infrastructure/kubernetes-delivery.md).

## Databricks and Modal

| Skill | Install source | Use when |
| --- | --- | --- |
| `databricks-model-serving` | `databricks/databricks-agent-skills` | Databricks serving endpoint lifecycle, canary or A/B routing, logs, metrics, permissions, AI Gateway limits, or streaming clients recur. |
| `modal-serverless-gpu` | `orchestra-research/ai-research-skills` | Modal hosts Python model APIs or GPU batch inference with on-demand resources and automatic scaling. |

For self-hosted runtimes and general endpoint benchmarks, open [model serving](serving.md). For provider infrastructure, open [cloud platforms](../infrastructure/cloud-platforms.md).
