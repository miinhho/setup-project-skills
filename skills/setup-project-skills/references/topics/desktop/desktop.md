# Desktop apps and embedded WebViews

| Skill | Install source | Use when |
| --- | --- | --- |
| `setting-up-tauri-projects` | `dchuk/claude-code-tauri-skills` | A new Tauri 2 project needs platform prerequisites and initialization. |
| `understanding-tauri-architecture` | `dchuk/claude-code-tauri-skills` | Tauri's Rust core, WebView shell, IPC, and security boundaries need design. |
| `understanding-tauri-process-model` | `dchuk/claude-code-tauri-skills` | Core, WebView, multiwindow, and process-isolation behavior affects a design or bug. |
| `configuring-tauri-apps` | `dchuk/claude-code-tauri-skills` | Tauri config, Cargo settings, or environment-specific application configuration recurs. |
| `calling-rust-from-tauri-frontend` | `dchuk/claude-code-tauri-skills` | Tauri frontend-to-Rust commands and IPC need focused guidance. |
| `calling-frontend-from-tauri-rust` | `dchuk/claude-code-tauri-skills` | Rust emits typed events or channels to the frontend. |
| `listening-to-tauri-events` | `dchuk/claude-code-tauri-skills` | Frontend event subscriptions and cleanup recur. |
| `configuring-tauri-capabilities` | `dchuk/claude-code-tauri-skills` | Per-window and platform capabilities need design. |
| `managing-tauri-plugin-permissions` | `dchuk/claude-code-tauri-skills` | Tauri capabilities or plugin permission scopes recur. |
| `configuring-tauri-scopes` | `dchuk/claude-code-tauri-skills` | Filesystem, URL, or command scopes need least-privilege configuration. |
| `configuring-tauri-csp` | `dchuk/claude-code-tauri-skills` | Tauri WebView content security policy needs configuration. |
| `integrating-tauri-js-frontends` | `dchuk/claude-code-tauri-skills` | Next.js, Nuxt, Qwik, SvelteKit, or Vite must run correctly as a Tauri frontend. |
| `running-nodejs-sidecar-in-tauri` | `dchuk/claude-code-tauri-skills` | A bundled Node.js process provides backend functionality. |
| `embedding-tauri-sidecars` | `dchuk/claude-code-tauri-skills` | External binaries are bundled and invoked across platforms. |
| `developing-tauri-plugins` | `dchuk/claude-code-tauri-skills` | A Tauri plugin, permission set, or mobile extension is implemented. |
| `managing-tauri-app-resources` | `dchuk/claude-code-tauri-skills` | Icons, bundled assets, resources, or runtime state recur. |
| `migrating-tauri-apps` | `dchuk/claude-code-tauri-skills` | A Tauri 1 or beta application migrates to Tauri 2 stable. |
| `debugging-tauri-apps` | `dchuk/claude-code-tauri-skills` | Tauri Rust or WebView DevTools diagnosis recurs. |
| `testing-tauri-apps` | `dchuk/claude-code-tauri-skills` | Tauri unit or WebDriver tests recur. |
| `building-tauri-with-github-actions` | `dchuk/claude-code-tauri-skills` | Cross-platform Tauri build and release workflows run in GitHub Actions. |
| `signing-tauri-apps` | `dchuk/claude-code-tauri-skills` | Tauri code signing or notarization recurs across release platforms. |
| `electron-best-practices` | [Electron skill subdirectory][electron-skill] | Electron process boundaries, IPC, preload security, packaging, and testing recur. |

For WebView work, select the skill for the host platform: Tauri WebView debugging or CSP above, [Swift WebKit](../languages/swift.md), or [Android](../mobile/android.md). For the embedded page and native bridge, open [WebView](../web/webview.md). For Qt or WinUI, open [native desktop](native.md). For interaction-based Electron QA, open [testing](../workflow/testing.md). Check the app's framework and version before proposing a skill.

[electron-skill]: https://github.com/jwynia/agent-skills/tree/main/skills/tech/development/tooling/electron-best-practices
