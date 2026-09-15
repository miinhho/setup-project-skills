# Native desktop frameworks

| Skill | Install source | Use when |
| --- | --- | --- |
| `qt-cmake-project` | `theqtcompanyrnd/agent-skills` | A Qt 6 CMake project, target, resource, or QML module needs setup. |
| `qt-ui-design` | `theqtcompanyrnd/agent-skills` | Qt Widgets or QML UI design recurs. |
| `qt-qml-test` | `theqtcompanyrnd/agent-skills` | QML interaction tests recur. |
| `winui-dev-workflow` | [WinUI workflow subdirectory][winui-workflow] | WinUI 3 build, run, or project setup recurs on Windows. |

For a Windows app's embedded WebView2, match the framework and its existing host API first. The WinUI workflow above assumes its documented Windows tooling; do not propose it for a Tauri or Electron project.

[winui-workflow]: https://github.com/microsoft/win-dev-skills/tree/main/plugins/winui/agent-plugin/skills/winui-dev-workflow
