# Contributing

🌐 Translations: [한국어](CONTRIBUTING.ko.md) (Community translation; may not reflect the latest updates.)

`setup-project-skills` helps coding agents find and select skills for a project's recurring work. This repository contains the setup procedure and a topic-based skill catalog.

## Find a topic to contribute to

Start with the [skill map](skills/setup-project-skills/references/skill-map.md) to find the technology or recurring work you want to contribute to.

1. Read the `Field` and `Open when` columns to identify the relevant topic.
2. Follow its `Map` link to review existing skill candidates, their sources, and use conditions.

## Evaluate skill candidates

Before adding an entry, read the candidate's `SKILL.md`, the references needed to assess it, and related candidates.

Consider:

- Which recurring work it addresses
- Whether its scope and activation conditions are clear
- Whether its version assumptions are compatible with the intended use
- Whether it provides actionable verification guidance
- Which tools or repository files it requires
- Whether its responsibilities overlap with existing candidates

Assess the actual content. When content quality is comparable, use maintainer or ecosystem-specialist provenance as supporting evidence. When retaining multiple candidates, their responsibilities should be distinct.

## What to record in the catalog

Each entry records the following information:

| Information | What to record |
| --- | --- |
| Skill name | The exact skill name |
| Installation source | An installable source |
| Work and use conditions | The work it addresses and when it is useful |
| Requirements | Any required tools or repository files |

See [SKILL.md](skills/setup-project-skills/SKILL.md) for the full discovery and comparison procedure.

## Pull request guidelines

- Write PR titles and descriptions in English.
- Follow the Conventional Commits format for PR titles. Include a scope when appropriate.
- Name branches using `<github-username>-patch-<number>`, where `github-username` is the contributor's GitHub username.

### Example

- PR title: `docs: add contribution guides`
- PR description: `Add English and Korean contribution guides.`
- Branch name: `octocat-patch-1`
