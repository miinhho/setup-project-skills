# PHP and Laravel

Read composer.json/lock, PHP/Laravel versions, installed packages, and project conventions first. Pennant guidance requires Pennant and its documentation tool; Laravel best practices also supports inspecting the installed framework if search-docs is unavailable.

| Skill | Install source | Use when |
| --- | --- | --- |
| `laravel-best-practices` | `laravel/boost` | Apply this skill whenever writing, reviewing, or refactoring Laravel PHP code. |
| `pennant-development` | `laravel/boost` | Laravel Pennant feature definitions, scoped checks, gradual rollouts, or feature-flag tests recur. |
| `starter-kit-upgrade` | `laravel/agent-skills` | Selectively pull upstream improvements from a Laravel starter kit (laravel/vue-starter-kit, laravel/react-starter-kit, laravel/svelte-starter-kit, laravel/livewire-starter-kit) into a project bootstrapped from one. |
| `deploying-to-cloud` | `laravel/agent-skills` | Deploys and manages Laravel applications on Laravel Cloud using the `cloud` CLI. |
| `configure-nightwatch` | `laravel/agent-skills` | Configures Laravel Nightwatch data collection, sampling rates, filtering rules, and redaction policies. |
| `laravel-tdd` | `affaan-m/ECC` | Laravel PHPUnit/Pest tests, factories, HTTP/database cases, or test-first implementation recur. |
| `laravel-security` | `affaan-m/ECC` | Laravel authentication, authorization, CSRF, mass assignment, uploads, or secret handling needs focused review. |
| `laravel-verification` | `affaan-m/ECC` | Laravel changes need an environment, formatting, static-analysis, test, and security verification loop. |

Cloud and Nightwatch candidates require the corresponding Laravel services and tools. Coding guidance, test strategy, security review, and verification are separate scopes; do not install all of them solely because Laravel is present.
