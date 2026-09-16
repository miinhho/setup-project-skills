# Security

| Skill                   | Install source                    | Use when                                                                                         |
| ----------------------- | --------------------------------- | ------------------------------------------------------------------------------------------------ |
| `security-review`       | `affaan-m/ECC`                    | A code change touches auth, user input, secrets, or sensitive data.                              |
| `security-threat-model` | `openai/skills`                   | A task explicitly needs an application threat model.                                             |
| `security-audit`        | `cloudflare/security-audit-skill` | A full codebase security audit, pen test, or vulnerability report with verified findings recurs. |

`security-audit` needs a sub-agent mechanism and Node.js for its bundled validators.
