# Infrastructure as code


| Skill                     | Install source                           | Use when                                                                            |
| ------------------------- | ---------------------------------------- | ----------------------------------------------------------------------------------- |
| `terraform-style-guide`   | `hashicorp/agent-skills`                 | Terraform configuration needs HashiCorp-maintained style and structure.             |
| `terraform-test`          | `hashicorp/agent-skills`                 | `.tftest.hcl`, mocks, run blocks, or module behavior tests recur.                   |
| `refactor-module`         | `hashicorp/agent-skills`                 | Monolithic Terraform configuration is split into reusable modules.                  |
| `terraform-search-import` | `hashicorp/agent-skills`                 | Existing cloud resources are discovered and imported into Terraform.                |
| `terraform-stacks`        | `hashicorp/agent-skills`                 | Terraform Stack components and deployments recur.                                   |
| `terraform-policy`        | `hashicorp/agent-skills`                 | Terraform Policy or policy tests recur.                                             |
| `new-terraform-provider`  | `hashicorp/agent-skills`                 | A new Terraform provider is scaffolded with the Plugin Framework.                   |
| `provider-resources`      | `hashicorp/agent-skills`                 | Terraform provider resources, data sources, CRUD, schema, import, or waiters recur. |
| `provider-test-patterns`  | `hashicorp/agent-skills`                 | Terraform provider acceptance tests recur.                                          |
| `opentofu-migration`      | `bagelhole/devops-security-agent-skills` | A Terraform project is evaluated or migrated to OpenTofu.                           |


Choose provider-development rows only for repositories that implement a Terraform provider. They do not belong in ordinary Terraform consumer projects.