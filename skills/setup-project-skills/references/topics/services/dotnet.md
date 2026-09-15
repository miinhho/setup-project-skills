# C# and .NET

Read the project SDK/TFMs, language version, frameworks, and recurring work before proposing skills. Open the section matching that work.

- [Language and runtime](#language-and-runtime)
- [ASP.NET Core and EF Core](#aspnet-core-and-ef-core)
- [Blazor](#blazor)
- [MAUI](#maui)
- [Build and packaging](#build-and-packaging)
- [Testing](#testing)
- [Performance and crash diagnostics](#performance-and-crash-diagnostics)

## Language and runtime

Read project SDK/TFMs and language versions first. Version migration candidates apply only to the stated source and destination; .NET 11 guidance applies only to a project intentionally targeting that release.

| Skill | Install source | Use when |
| --- | --- | --- |
| `csharp-scripts` | `dotnet/skills` | Run file-based C# apps with the .NET CLI when the user explicitly wants C#/.NET code without creating a project. |
| `dotnet-pinvoke` | `dotnet/skills` | Correctly call native (C/C++) libraries from .NET using P/Invoke and LibraryImport. |
| `vectorization` | `dotnet/skills` | Design, implement, optimize, and review SIMD code in .NET. |
| `dotnet-aot-compat` | `dotnet/skills` | Make .NET projects compatible with Native AOT and trimming by systematically resolving IL trim/AOT analyzer warnings. |
| `migrate-nullable-references` | `dotnet/skills` | Enable nullable reference types in a C# project and systematically resolve all warnings. |
| `migrate-dotnet8-to-dotnet9` | `dotnet/skills` | Migrate a .NET 8 project to .NET 9 and resolve all breaking changes. |
| `migrate-dotnet9-to-dotnet10` | `dotnet/skills` | Migrate a .NET 9 project or solution to .NET 10 and resolve all breaking changes. |
| `migrate-dotnet10-to-dotnet11` | `dotnet/skills` | Migrate a .NET 10 project or solution to .NET 11 and resolve all breaking changes. |
| `thread-abort-migration` | `dotnet/skills` | Guides migration of .NET Framework Thread.Abort usage to cooperative cancellation in modern .NET. |
| `system-text-json-net11` | `dotnet/skills` | A .NET 11 project uses new System.Text.Json naming-policy or typed metadata APIs. |

## ASP.NET Core and EF Core

Match the project's controller/minimal API, ORM, and hosting conventions. EF Core-specific candidates apply to EF Core data access; they do not justify adopting an ORM.

| Skill | Install source | Use when |
| --- | --- | --- |
| `dotnet-webapi` | `dotnet/skills` | Guides creation and modification of ASP.NET Core Web API endpoints with correct HTTP semantics, OpenAPI metadata, and error handling. |
| `minimal-api-file-upload` | `dotnet/skills` | File upload endpoints in ASP.NET minimal APIs (.NET 8+) |
| `optimizing-ef-core-queries` | `dotnet/skills` | Optimize and improve the performance of slow Entity Framework Core (EF Core) queries: make them generate less SQL, make fewer database round-trips, and return results faster. |
| `create-datadriven-aspnetcore` | `dotnet/skills` | Generate or scaffold ASP.NET Core code — Razor Pages, Blazor components, MVC controllers, views, and Minimal API endpoints — without using ASP.NET Core CLI scaffolding/code-generation tools. |

## Blazor

Identify static SSR, Interactive Server, WebAssembly, or Auto render mode before proposing a skill. State sharing, prerender persistence, authentication, and interop have different lifecycle constraints.

| Skill | Install source | Use when |
| --- | --- | --- |
| `create-blazor-project` | `dotnet/skills` | Create a new ASP.NET Core web application or web site using Blazor. |
| `collect-user-input` | `dotnet/skills` | Build forms, validate data, and react to user input in Blazor. |
| `configure-auth` | `dotnet/skills` | Add authentication and authorization to a Blazor Web App, accounting for the app's render mode. |
| `coordinate-components` | `dotnet/skills` | Share state between components that don't have a direct parent-child parameter relationship, using cascading values, scoped services with change events, or CascadingValueSource via DI. |
| `fetch-and-send-data` | `dotnet/skills` | Call APIs, load data into components, and handle the async lifecycle in Blazor. |
| `plan-ui-change` | `dotnet/skills` | Plan complex Blazor UI features by decomposing them into focused components. |
| `support-prerendering` | `dotnet/skills` | Make interactive Blazor components work correctly with prerendering. |
| `use-js-interop` | `dotnet/skills` | Add, review, or fix JavaScript interop in Blazor components. |
| `convert-blazor-server-to-webapp` | `dotnet/skills` | Guides conversion of a pre-.NET 8 Blazor Server app into a .NET 8+ Blazor Web App. |

## MAUI

Match the target platforms, MAUI version, installed workloads, and XAML/MVVM conventions. Safe-area guidance has its own version boundary.

| Skill | Install source | Use when |
| --- | --- | --- |
| `dotnet-maui-doctor` | `dotnet/skills` | MAUI SDK, workloads, JDK, Android SDK, Xcode, or Windows SDK setup needs diagnosis. |
| `maui-app-lifecycle` | `dotnet/skills` | MAUI activation, suspension, resume, destruction, or cross-platform Window lifecycle handling recurs. |
| `maui-collectionview` | `dotnet/skills` | Guidance for implementing CollectionView in .NET MAUI apps — data display, layouts (list & grid), selection, grouping, scrolling, empty views, templates, incremental loading, swipe actions, and pull-to-refresh. |
| `maui-data-binding` | `dotnet/skills` | Guidance for .NET MAUI XAML and C# data bindings — compiled bindings, INotifyPropertyChanged / ObservableObject, value converters, binding modes, multi-binding, relative bindings, fallbacks, and MVVM best practices. |
| `maui-dependency-injection` | `dotnet/skills` | MAUI service registration, lifetimes, Shell resolution, or platform-specific dependencies recur. |
| `maui-safe-area` | `dotnet/skills` | .NET MAUI safe area and edge-to-edge layout guidance for .NET 10+. |
| `maui-shell-navigation` | `dotnet/skills` | Guide for implementing Shell-based navigation in .NET MAUI apps. |
| `maui-theming` | `dotnet/skills` | Guide for theming .NET MAUI apps — light/dark mode via AppThemeBinding, ResourceDictionary theme switching, DynamicResource bindings, system theme detection, and user theme preferences. |

## Build and packaging

Choose the build, packaging, or template operation that recurs. SDK and package publication candidates may change environments or external services; the setup proposal must describe those prerequisites separately from skill installation.

| Skill | Install source | Use when |
| --- | --- | --- |
| `setup-local-sdk` | `dotnet/skills` | Install a .NET SDK locally for safe preview testing, specific-version pinning, or reproducible team setups — without modifying the system-wide installation. |
| `nuget-trusted-publishing` | `dotnet/skills` | Set up NuGet trusted publishing (OIDC) on a GitHub Actions repo — replaces long-lived API keys with short-lived tokens. |
| `convert-to-cpm` | `dotnet/skills` | Convert .NET projects and solutions (.sln, .slnx) to NuGet Central Package Management (CPM) using Directory.Packages.props. |
| `binlog-failure-analysis` | `dotnet/skills` | Analyze MSBuild binary logs to diagnose build failures. |
| `binlog-generation` | `dotnet/skills` | Generate MSBuild binary logs (binlogs) for build diagnostics and analysis. |
| `build-parallelism` | `dotnet/skills` | Diagnose and fix under-parallelized MSBuild builds. |
| `build-perf-baseline` | `dotnet/skills` | Establish build performance baselines and apply systematic optimization techniques. |
| `build-perf-diagnostics` | `dotnet/skills` | Diagnose MSBuild build performance bottlenecks using binary log analysis. |
| `check-bin-obj-clash` | `dotnet/skills` | Detects MSBuild projects with conflicting OutputPath or IntermediateOutputPath. |
| `directory-build-organization` | `dotnet/skills` | Guide for organizing MSBuild infrastructure with Directory.Build.props, Directory.Build.targets, Directory.Packages.props, and Directory.Build.rsp. |
| `incremental-build` | `dotnet/skills` | Guide for optimizing MSBuild incremental builds. |
| `including-generated-files` | `dotnet/skills` | Fix MSBuild targets that generate files during the build but those files are missing from compilation or output. |
| `item-management` | `dotnet/skills` | Patterns for managing MSBuild item groups: Include/Remove/Update semantics, item metadata, batching with %(Metadata), transforms, per-item filtering, and cross-product batching pitfalls. |
| `msbuild-antipatterns` | `dotnet/skills` | Detect and fix MSBuild anti-patterns in project and build files. |
| `msbuild-modernization` | `dotnet/skills` | Guide for modernizing and migrating MSBuild project files to SDK-style format. |
| `property-patterns` | `dotnet/skills` | MSBuild property definition patterns: conditional defaults, composition/concatenation, path normalization, trailing-slash handling, TFM detection helpers, and evaluation order. |
| `resolve-project-references` | `dotnet/skills` | MSBuild ResolveProjectReferences timing appears dominant and needs interpretation before optimization. |
| `target-authoring` | `dotnet/skills` | Canonical patterns for writing custom MSBuild targets. |
| `extension-points` | `dotnet/skills` | Custom MSBuild imports, before/after hooks, or NuGet build/buildTransitive integration recur. |
| `copy-to-output-directory` | `dotnet/skills` | Choosing an MSBuild CopyToOutputDirectory / CopyToPublishDirectory mode: Never, PreserveNewest, Always, and IfDifferent (MSBuild 17.13+), plus $(SkipUnchangedFilesOnCopyAlways). |
| `eval-performance` | `dotnet/skills` | Guide for diagnosing and improving MSBuild project evaluation performance. |
| `template-authoring` | `dotnet/skills` | Guides creation and validation of custom dotnet new templates from existing projects. |
| `template-comparison` | `dotnet/skills` | Compares two or more dotnet new templates side by side to help users choose between them based on parameters, feature support, frameworks, and classifications. |
| `template-discovery` | `dotnet/skills` | Helps find, inspect, and compare (at a high level) .NET project templates. |
| `template-instantiation` | `dotnet/skills` | Creates .NET projects from templates with validated parameters, smart defaults, Central Package Management adaptation, and latest NuGet version resolution. |
| `template-smart-defaults` | `dotnet/skills` | Applies cross-parameter default rules when creating .NET projects with dotnet new, filling gaps consistently without overriding values the user set explicitly. |
| `template-validation` | `dotnet/skills` | Validates custom dotnet new templates for correctness before publishing. |

## Testing

Identify the existing framework and runner before proposing test guidance or migration. Runner migration and framework conversion are distinct. Keep the current framework unless a conversion is requested; select coverage or testability analysis only for recurring needs.

| Skill | Install source | Use when |
| --- | --- | --- |
| `run-tests` | `dotnet/skills` | Exact .NET test execution commands must match the existing runner, framework, filter, and build state. |
| `filter-syntax` | `dotnet/skills` | Known VSTest/MTP and test-framework filters need creation or translation. |
| `platform-detection` | `dotnet/skills` | Identify a .NET project's test platform, framework, command mode, and SDK-style vs classic project system. |
| `scaffold-dotnet-test-project` | `dotnet/skills` | A .NET test project needs scaffolding, solution registration, CI discovery, or restored production references. |
| `writing-mstest-tests` | `dotnet/skills` | ALWAYS USE when asked to fix, rewrite, update, improve, modernize, show corrected code for, or explain existing MSTest tests or MSTest-specific configuration. |
| `test-tagging` | `dotnet/skills` | Classifies existing tests by standard traits and reports their distribution. |
| `assertion-quality` | `dotnet/skills` | Existing .NET tests have weak, tautological, missing, or insufficiently discriminating assertions. |
| `coverage-analysis` | `dotnet/skills` | Activation requires either supplied .NET coverage reports/percentages/line, branch, or condition metrics, or an explicit request to collect .NET coverage for analysis. |
| `find-untested-sources` | `dotnet/skills` | MANDATORY for static source-to-test pairing: find or list source files/modules without corresponding tests, or suggest test locations from repository structure. |
| `test-gap-analysis` | `dotnet/skills` | Existing .NET assertions need analysis of meaningful production mutations they would miss. |
| `test-smell-detection` | `dotnet/skills` | Audits existing tests in any language using formal, research-backed test smell names and the testsmells.org 19-smell academic taxonomy. |
| `test-anti-patterns` | `dotnet/skills` | A .NET test suite needs a ranked review for empty verification, flakiness, exceptions, or duplication. |
| `detect-static-dependencies` | `dotnet/skills` | ACTIVATION PREREQUISITE: the request or discovered target must explicitly identify C#, .NET, `.cs`, or `.csproj`; otherwise stay dormant without invoking this skill. |
| `testability-obstacle` | `dotnet/skills` | MUST USE for C#/.NET deterministic tests that require the smallest production seam for DateTime/Task.Delay/File/Environment/Guid/Random, static API preservation, nested/parallel overrides, or no real I/O. |
| `migrate-mstest-v1v2-to-v3` | `dotnet/skills` | An MSTest v1/v2 project is intentionally migrating to v3 or repairing that migration. |
| `migrate-mstest-v3-to-v4` | `dotnet/skills` | An MSTest v3 project is intentionally migrating to v4 or fixing v4 breaking changes. |
| `migrate-vstest-to-mtp` | `dotnet/skills` | A test runner or CI pipeline is intentionally migrating from VSTest to Microsoft.Testing.Platform. |
| `migrate-xunit-to-xunit-v3` | `dotnet/skills` | Migrate .NET test projects from xUnit.net v2 to xunit.v3 and fix v3 breaks. |
| `migrate-xunit-to-mstest` | `dotnet/skills` | Convert .NET tests from xUnit.net v2/v3 to MSTest v4 while preserving VSTest or MTP. |
| `migrate-nunit-to-mstest` | `dotnet/skills` | Convert .NET tests from NUnit 3/4 to MSTest v4 while preserving VSTest or MTP. |

## Performance and crash diagnostics

Choose static analysis, measurement, artifact capture, native symbolication, or instrumentation according to the actual investigation. Android and Apple candidates apply to native .NET runtime frames, not unrelated Kotlin/Swift crashes.

| Skill | Install source | Use when |
| --- | --- | --- |
| `analyzing-dotnet-performance` | `dotnet/skills` | Scans .NET code for ~50 performance anti-patterns across async, memory, strings, collections, LINQ, regex, serialization, and I/O with tiered severity classification. |
| `microbenchmarking` | `dotnet/skills` | BenchmarkDotNet cases, comparison axes, execution cost, or measurement validity need guidance. |
| `dotnet-trace-collect` | `dotnet/skills` | Guide developers through capturing diagnostic artifacts to diagnose production .NET performance issues. |
| `dump-collect` | `dotnet/skills` | Configure and collect crash dumps for modern .NET applications. |
| `android-tombstone-symbolication` | `dotnet/skills` | Android tombstones contain .NET native runtime frames needing symbolication. |
| `apple-crash-symbolication` | `dotnet/skills` | Apple .ips crash logs contain .NET native runtime frames needing dSYM/atos symbolication. |
| `clr-activation-debugging` | `dotnet/skills` | Diagnoses .NET Framework CLR activation issues using CLR activation logs (CLRLoad logs) produced by mscoree.dll. |
| `configuring-opentelemetry-dotnet` | `dotnet/skills` | Configure OpenTelemetry distributed tracing, metrics, and logging in ASP.NET Core using the .NET OpenTelemetry SDK. |
