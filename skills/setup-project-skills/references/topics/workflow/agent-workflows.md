# Agent workflows

| Skill | Install source | Use when |
| --- | --- | --- |
| `agent-harness-construction` | `affaan-m/ECC` | Agent tools, action space, or observation format need design. |
| `agent-eval` | `affaan-m/ECC` | Agent changes need task-level pass-rate, time, and cost comparisons. |
| `parallel-feature-development` | `wshobson/agents` | A harness already supports parallel implementers and needs one owner per file, shared contract ownership, decomposition choices, and integration handoffs. |
| `parallel-debugging` | `wshobson/agents` | A harness supports independent investigators and a difficult bug needs competing hypotheses, source-backed evidence, result arbitration, and reproduction-based fix verification. |
| `multi-reviewer-patterns` | `wshobson/agents` | A harness supports multiple reviewers and needs change-specific review dimensions, finding deduplication, severity criteria, and consolidated reporting. |
| `mcp-builder` | `anthropics/skills` | The project repeatedly builds MCP servers for external services. |
| `mcp-server-patterns` | `affaan-m/ECC` | A TypeScript MCP server needs tools, resources, prompts, Zod validation, and transport guidance. |
| `a2a-cli` | `a2aproject/a2a-cli` | A harness must discover or interact with A2A agents through the official CLI. |
| `google-agents-cli-adk-code` | `google/agents-cli` | Google ADK agent implementation recurs. |
| `google-agents-cli-eval` | `google/agents-cli` | Google ADK agents need repeatable evaluations. |
| `ai-sdk` | `vercel/ai` | Vercel AI SDK integration recurs. |
| `claude-api` | `anthropics/skills` | Anthropic SDK or Claude API integration recurs. |
| `building-pydantic-ai-agents` | `pydantic/skills` | PydanticAI agents or tools recur. |
| `pydantic-ai-harness` | `pydantic/skills` | A PydanticAI agent needs code mode, sandboxed filesystem and shell, subagents, planning, or compaction. |
| `agents-sdk` | [OpenAI Agents SDK skill][openai-agents-sdk] | OpenAI Agents SDK apps or evaluations recur; verify its companion API-key workflow before proposing installation. |
| `langfuse` | `langfuse/skills` | LLM tracing and evaluation through Langfuse recur. |
| `langchain-fundamentals` | `langchain-ai/langchain-skills` | LangChain agent and model integrations recur. |
| `langchain-dependencies` | `langchain-ai/langchain-skills` | LangChain, LangGraph, LangSmith, or Deep Agents package versions and setup recur. |
| `langchain-middleware` | `langchain-ai/langchain-skills` | LangChain human approval, structured output, error handling, or custom middleware recurs. |
| `langgraph-fundamentals` | `langchain-ai/langchain-skills` | A LangGraph project uses explicit state, nodes, edges, Command, Send, or streaming. |
| `langgraph-persistence` | `langchain-ai/langchain-skills` | LangGraph checkpointers, thread state, memory, time travel, or subgraph persistence recur. |
| `langgraph-human-in-the-loop` | `langchain-ai/langchain-skills` | LangGraph pauses for approval, validation, or recoverable error handling. |
| `deep-agents-core` | `langchain-ai/langchain-skills` | A Deep Agents application needs its harness, tools, skills, and backend configured. |
| `deep-agents-memory` | `langchain-ai/langchain-skills` | A Deep Agent needs ephemeral, persistent, filesystem, or composite memory. |
| `deep-agents-orchestration` | `langchain-ai/langchain-skills` | Deep Agents uses subagents, task planning, or human approval. |
| `eval-engineering` | `langchain-ai/langchain-skills` | Agent benchmarks need task specs, controlled environments, verifiers, or calibration. |
| `mcp-server-offering` | `samber/developer-platform-skills` | A SaaS product needs an MCP surface, tool curation, OAuth, write safety, versioning, and adoption metrics designed before implementation. |

For retrieval pipelines and evaluation, open [RAG](../ai/rag.md).

[openai-agents-sdk]: https://github.com/openai/plugins/tree/main/plugins/openai-developers/skills/agents-sdk
