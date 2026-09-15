# setup-project-skills

`setup-project-skills` helps your coding agent find and install skills for a repository. It includes a catalog of individual skills, organized by topic, and instructions for choosing a set that fits your project's recurring work.

Skills give an agent instructions for tasks such as reviewing SQL queries or testing browser flows. During setup, the agent reads candidate skills, compares their scope and requirements, and asks you to approve specific additions.

## What to expect

1. The agent inspects the repository's stack, versions, recurring tasks, tests, and existing skills and instructions.
2. It reads the relevant catalog topics and related skills from each source, then searches further if it finds gaps.
3. You receive a proposal with exact skill names and sources, the work each addresses, the comparison with overlapping candidates, and the files or configuration that would change.
4. After you approve the additions, the agent installs them in the target project by default.
5. It checks that it can access the installed skills and reports the changes.

For a PostgreSQL project, the agent might propose a query optimization skill to help investigate slow queries. Migration and deployment skills need their own use cases to justify inclusion.

You can rerun setup as the project changes. The agent compares proposed additions or updates with existing skills and preserves your customizations.

## Browse the catalog

Start with the [skill map](skills/setup-project-skills/references/skill-map.md). It links to topic files where each entry gives a skill's name, installation source, and use conditions. The agent opens the topics that match your project.


| Area                 | Examples                                                                  |
| -------------------- | ------------------------------------------------------------------------- |
| Languages            | Python, TypeScript, Go, Rust, Java, Kotlin, Swift, C and C++              |
| Web and services     | React, Next.js, CSS, Spring Boot 4, .NET, authentication and APIs         |
| AI                   | Model training and evaluation, RAG, local and managed serving             |
| Databases            | PostgreSQL, MySQL, Redis, MongoDB, analytical, vector and graph databases |
| Data engineering     | DataFrames, Spark, Airflow, Dagster and streaming pipelines               |
| Mobile and desktop   | React Native, Expo, Flutter, Android, Tauri and Electron                  |
| Infrastructure       | Containers, Kubernetes, cloud platforms, IaC, observability and security  |
| Workflows            | Testing, QA, architecture, planning, reviews and agent development        |
| Systems and graphics | CUDA, HPC, WebAssembly, Linux, game engines and web graphics              |


This repository stores the catalog and setup instructions. The agent fetches external skills from their sources during installation and checks their current availability and content during setup. Topic files describe any special installation method, including TanStack Intent.

## Add or improve a topic

Start with the [skill map](skills/setup-project-skills/references/skill-map.md) and the corresponding file under `skills/setup-project-skills/references/topics/`.

Read the skill and related candidates before adding an entry. Record its exact name, an installable source, the work it addresses, and any required tools or repository files. Compare overlapping skills for version compatibility, scope, and verification guidance. A maintainer's skill may be a good starting point; assess its content alongside other candidates.

See the [setup instructions](skills/setup-project-skills/SKILL.md) for the full procedure.
