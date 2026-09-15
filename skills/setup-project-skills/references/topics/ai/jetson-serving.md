# Jetson model serving

Match the Jetson SKU, JetPack/L4T release, available memory, serving-runtime build, and access to the device. Memory tuning uses a `jetson-memory-audit` snapshot. Its audit script calls `jetson-diagnostic/scripts/snapshot.sh` by a sibling path; keep both skills and their bundled scripts in the same installed skills directory when collecting that snapshot.

## Runtime and memory

| Skill | Install source | Use when |
| --- | --- | --- |
| `jetson-llm-serve` | `NVIDIA/skills` | A Jetson LLM/VLM endpoint needs the validated vLLM or SGLang runtime/image for its Thor or Orin JetPack/L4T combination and server verification. |
| `jetson-diagnostic` | `NVIDIA/skills` | Jetson serving or memory audits need the source's host identity, DRAM/NvMap, GPU, thermal, and process snapshot collector. |
| `jetson-memory-audit` | `NVIDIA/skills` | Jetson serving needs a live DRAM/NvMap baseline or before/after memory verification rather than estimates from model or container size. |
| `jetson-inference-mem-tune` | `NVIDIA/skills` | A measured Jetson workload needs a serving stack and per-runtime memory flags to fit a model, reduce OOM risk, or use a lower-memory runtime. |

## Measurement and decode tuning

| Skill | Install source | Use when |
| --- | --- | --- |
| `jetson-llm-benchmark` | `NVIDIA/skills` | Jetson vLLM, llama.cpp, or Ollama serving needs structured throughput, TTFT, TPOT, or latency measurements. |
| `jetson-speculative-decoding` | `NVIDIA/skills` | A working Thor or AGX Orin vLLM server has a measured low-concurrency decode bottleneck, compatible EAGLE-3 or draft-model support, and enough memory headroom for a before/after experiment. |

Speculative decoding needs a working `jetson-llm-serve` configuration and a `jetson-llm-benchmark` baseline. Follow the source's SKU and memory restrictions when shortlisting it; a generic Jetson dependency does not establish a fit.

For GGUF selection, general runtime configuration, or other serving benchmarks, open [model serving](serving.md). For CUDA kernels and GPU profiling, open [CUDA and GPU acceleration](../systems/cuda.md).
