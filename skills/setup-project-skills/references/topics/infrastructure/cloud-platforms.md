# Cloud platforms

## AWS

| Skill | Install source | Use when |
| --- | --- | --- |
| `aws-cdk` | `aws/agent-toolkit-for-aws` | CDK stacks and constructs in TypeScript or Python recur. |
| `aws-cloudformation` | `aws/agent-toolkit-for-aws` | CloudFormation authoring, validation, change sets, or failed-stack diagnosis recurs. |
| `aws-containers` | `aws/agent-toolkit-for-aws` | EKS, ECS, Fargate, ECR, or Karpenter work recurs. |
| `aws-serverless` | `aws/agent-toolkit-for-aws` | Lambda, API Gateway, Step Functions, EventBridge, or SAM work recurs. |
| `aws-deployment` | `aws/agent-toolkit-for-aws` | CodePipeline, CodeBuild, CodeDeploy, or CodeArtifact delivery recurs. |
| `aws-iam` | `aws/agent-toolkit-for-aws` | IAM policy evaluation, trust, STS, roles, or least privilege recur. |
| `aws-observability` | `aws/agent-toolkit-for-aws` | CloudWatch, X-Ray, CloudTrail, ADOT, or Application Signals recur. |
| `aws-storage` | `aws/agent-toolkit-for-aws` | S3, EBS, EFS, FSx, archival, replication, or storage selection recurs. |

## Azure

| Skill | Install source | Use when |
| --- | --- | --- |
| `azure-app-onboard-prereq` | `microsoft/azure-skills` | An application needs readiness and compatibility checks before Azure infrastructure work. |
| `azure-prepare` | `microsoft/azure-skills` | An azd-based project needs `azure.yaml`, Bicep/Terraform, or container preparation. |
| `azure-validate` | `microsoft/azure-skills` | Azure configuration, IaC, RBAC, identity, or deployment prerequisites need validation. |
| `azure-deploy` | `microsoft/azure-skills` | An already prepared Azure project is deployed through azd. |
| `azure-kubernetes` | `microsoft/azure-skills` | AKS planning, networking, identity, security, or operations recur. |
| `python-appservice-deploy` | `microsoft/azure-skills` | Flask, Django, or FastAPI deploys to Azure App Service Linux. |

## Google Cloud

| Skill | Install source | Use when |
| --- | --- | --- |
| `finding-google-skills` | `google/skills` | A Google or GCP project needs routing to a current product-specific official skill. |
| `gcloud` | `google/skills` | gcloud commands need validation, guardrails, and reduced output. |
| `cloud-run-basics` | `google/skills` | Cloud Run services, jobs, or worker pools recur. |
| `google-cloud-storage-basics` | `google/skills` | Cloud Storage buckets and objects are managed from application or CLI workflows. |

For official GKE foundation, networking, workload/node/identity diagnosis, or backup skills, open [GKE](gke.md).

## Edge and application platforms

| Skill | Install source | Use when |
| --- | --- | --- |
| `cloudflare` | `cloudflare/skills` | A Cloudflare project needs product selection and routing to a focused official skill. |
| `workers-best-practices` | `cloudflare/skills` | Cloudflare Workers implementation or configuration recurs. |
| `durable-objects` | `cloudflare/skills` | Durable Objects own persistent state or coordination. |
| `wrangler` | `cloudflare/skills` | Wrangler commands and Worker resource configuration recur. |
| `nextjs-on-cloudflare` | `cloudflare/skills` | Next.js runs or migrates to Cloudflare Workers. |
| `agents-sdk` | `cloudflare/skills` | Cloudflare Agents SDK applications recur. |
| `turnstile-spin` | `cloudflare/skills` | Turnstile client and server verification recurs. |
| `deploy-to-vercel` | `vercel-labs/agent-skills` | Preview or production deployment to Vercel recurs. |
| `vercel-cli-with-tokens` | `vercel-labs/agent-skills` | Vercel CLI automation uses token authentication. |
| `vercel-optimize` | `vercel-labs/agent-skills` | Vercel cost or performance work is based on deployed metrics. |
| `deno-deploy` | `denoland/skills` | A Deno project deploys to Deno Deploy. |
| `temporal-developer` | `temporalio/skill-temporal-developer` | Temporal workflows and activities recur. |
