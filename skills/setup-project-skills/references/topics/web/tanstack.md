# TanStack package skills through Intent

Use [TanStack Intent](https://tanstack.com/intent/latest/docs/getting-started/quick-start-consumers) to inspect skills shipped with installed TanStack dependency versions.

1. Inspect TanStack dependencies and the lockfile. From the target project root, run `npx @tanstack/intent@latest list --json` to see available package-version skills. Inspect relevant skill content and existing `package.json#intent` permissions and `AGENTS.md` guidance.
2. Include only useful package/skill names and the expected Intent configuration changes in the setup proposal. Let the main skill obtain approval before running a command that writes to the project.
3. After approval, run `npx @tanstack/intent@latest install` if setup is needed. Permit only the approved packages or skills, preserve existing guidance, and review the resulting diff. Run `npx @tanstack/intent@latest hooks install` only if that specific Codex hook setup was also approved.
4. Verify selected names with `npx @tanstack/intent@latest list`. Load a chosen skill with `npx @tanstack/intent@latest load <package>#<skill>` when its task arises. Record the installed dependency versions and Intent allowlist as the source record; recheck them after dependency updates.
