# Elixir, OTP, Ecto, and Phoenix

Implementation advice, macro construction, paradigm review, BEAM runtime review, and LiveView lifecycle review are separate roles. Review gates require subagent support; confirm that the target harness can run their reviewer contract. These candidates live in the source's experimental collection.

| Skill | Install source | Use when |
| --- | --- | --- |
| `staff-level-elixir` | `pproenca/dot-skills` | OTP process ownership, bounded concurrency, Ecto transactions, or Phoenix boundaries need implementation guidance. |
| `elixir-meta-programming` | `pproenca/dot-skills` | A justified Elixir macro or declarative DSL needs quote hygiene, single evaluation, and compile-time validation. |
| `adversarial-elixir` | `pproenca/dot-skills` | Elixir/OTP code needs a blind pass/fail review for foreign architecture patterns. |
| `adversarial-beam` | `pproenca/dot-skills` | BEAM supervision, failure handling, message delivery, or backpressure needs a blind pass/fail review. |
| `adversarial-phoenix-liveview` | `pproenca/dot-skills` | LiveView socket state, mount lifecycle, streams, events, or context boundaries need a blind pass/fail review. |
