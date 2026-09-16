# Security

| Skill                   | Install source                    | Use when                                                                                         |
| ----------------------- | --------------------------------- | ------------------------------------------------------------------------------------------------ |
| `security-review`       | `affaan-m/ECC`                    | A code change touches auth, user input, secrets, or sensitive data.                              |
| `security-threat-model` | `openai/skills`                   | A task explicitly needs an application threat model.                                             |
| `security-audit`        | `cloudflare/security-audit-skill` | A full codebase security audit, pen test, or vulnerability report with verified findings recurs. |

`security-audit` runs a six-phase audit (reconnaissance, coverage-led hunting, candidate validation, structured output, record verification, reporting) through isolated sub-agents, so it needs a platform with a delegation or sub-agent mechanism and Node.js for its zero-dependency validators. It writes audit artifacts to a directory outside the target repository and defaults to guidance mode for focused security questions.
