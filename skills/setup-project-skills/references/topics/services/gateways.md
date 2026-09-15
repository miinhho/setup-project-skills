# API gateways


| Skill                             | Install source        | Use when                                                                                              |
| --------------------------------- | --------------------- | ----------------------------------------------------------------------------------------------------- |
| `deck-gateway`                    | `kong/ai-marketplace` | Kong Gateway entities are managed with decK state, validate, diff, sync, dump, or OpenAPI generation. |
| `gateway-plugin-datakit`          | `kong/ai-marketplace` | Kong DataKit plugin DAGs, jq transformations, cache, vault, or phase behavior recur.                  |
| `kongctl-declarative`             | `kong/ai-marketplace` | Konnect resources are managed through declarative kongctl YAML and plan, diff, apply, or sync.        |
| `kongctl-query`                   | `kong/ai-marketplace` | Read-only kongctl discovery, authentication, scope, or JSON/YAML inspection recurs.                   |
| `konnect-access-scope`            | `kong/ai-marketplace` | Konnect authentication, region, organization, team, role, or resource-visibility failures recur.      |
| `konnect-ai-gateway`              | `kong/ai-marketplace` | Konnect AI Gateway provider routing, AI Proxy, controls, or LLM analytics recur.                      |
| `konnect-api-catalog`             | `kong/ai-marketplace` | Konnect API Catalog APIs, versions, specs, implementations, or packages recur.                        |
| `konnect-api-publish`             | `kong/ai-marketplace` | APIs are published from Konnect Catalog to a Dev Portal with audience scoping.                        |
| `konnect-app-auth`                | `kong/ai-marketplace` | Konnect Dev Portal application registration, approval, credentials, or auth strategies recur.         |
| `konnect-control-plane-bootstrap` | `kong/ai-marketplace` | A new Konnect control plane needs topology, region, naming, ownership, or data-plane bootstrap.       |
| `konnect-event-gateway`           | `kong/ai-marketplace` | Konnect Event Gateway listeners, hostnames, clusters, auth, or policy behavior recur.                 |
| `konnect-gateway-triage`          | `kong/ai-marketplace` | Konnect control-plane, data-plane, rollout, drift, network, or traffic failures need diagnosis.       |
| `konnect-monetization`            | `kong/ai-marketplace` | Konnect meters, features, plans, rate cards, allowances, or invoices recur.                           |
| `konnect-observability-triage`    | `kong/ai-marketplace` | Konnect Analytics, Explorer, or Debugger data is missing, delayed, or mis-scoped.                     |
| `konnect-platform-router`         | `kong/ai-marketplace` | A project repeatedly spans several Konnect surfaces and needs routing to the owning workflow.         |
| `portal-branding`                 | `kong/ai-marketplace` | A Konnect Dev Portal must reproduce an existing brand through MDC components and page styles.         |
| `portal-page-design`              | `kong/ai-marketplace` | Konnect Dev Portal page layout and MDC component composition recur.                                   |
| `terraform-kong-gateway`          | `kong/ai-marketplace` | Terraform manages self-hosted Kong Gateway Admin API entities.                                        |
| `terraform-konnect`               | `kong/ai-marketplace` | Terraform manages Konnect resources, imports, plans, or applies.                                      |


For Spring Cloud Gateway, open [Spring Boot 4](spring.md). For Kubernetes ingress and service-mesh routing, open [Kubernetes and delivery](../infrastructure/kubernetes-delivery.md).