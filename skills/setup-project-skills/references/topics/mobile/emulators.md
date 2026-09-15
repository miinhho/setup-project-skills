# Mobile emulators and device QA

| Skill | Install source | Use when |
| --- | --- | --- |
| `android-emulator` | `callstack/agent-device` | Android emulator interaction and visual QA recur. Requires the separate `agent-device` CLI. |
| `ios-simulator` | `callstack/agent-device` | iOS Simulator interaction and visual QA recur. Requires the separate `agent-device` CLI and a compatible host. |
| `eas-simulator` | `expo/skills` | An Expo/EAS project needs an agent-controlled remote iOS or Android simulator. Requires the paid experimental EAS service. |

These are runtime QA tools, not substitutes for the project's widget, unit, or integration tests. Confirm tool and host prerequisites before proposing them for installation.
