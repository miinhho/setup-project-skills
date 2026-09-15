# Machine learning and model evaluation


| Skill                               | Install source                        | Use when                                                                                                                |
| ----------------------------------- | ------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `mle-workflow`                      | `affaan-m/ECC`                        | Reproducible training, evaluation, deployment, or monitoring recur.                                                     |
| `pytorch-patterns`                  | `affaan-m/ECC`                        | PyTorch training loops, data loading, reproducibility, or model architecture recur.                                     |
| `pytorch-lightning`                 | `k-dense-ai/scientific-agent-skills`  | LightningModules, Trainer configuration, callbacks, or distributed PyTorch training recur.                              |
| `tensorflow-deep-learning`          | `mindrally/skills`                    | TensorFlow/Keras data pipelines, training, evaluation, or model export recurs.                                          |
| `scikit-learn`                      | `k-dense-ai/scientific-agent-skills`  | scikit-learn pipelines, preprocessing, model selection, or validation recur.                                            |
| `transformers`                      | `k-dense-ai/scientific-agent-skills`  | Hugging Face Transformers loading, pipeline inference, tokenizers, or Trainer work recurs.                              |
| `hf-cli`                            | `huggingface/skills`                  | Hugging Face Hub models, datasets, Spaces, Jobs, endpoints, cache, or repositories are managed through `hf`.            |
| `huggingface-datasets`              | `huggingface/skills`                  | Dataset Viewer API queries or dataset inspection recur.                                                                 |
| `huggingface-llm-trainer`           | `huggingface/skills`                  | Language or vision models train on Hugging Face Jobs with TRL or Unsloth.                                               |
| `huggingface-vision-trainer`        | `huggingface/skills`                  | Detection, classification, or SAM/SAM2 training on Hugging Face Jobs recurs.                                            |
| `trl-training`                      | `huggingface/skills`                  | Local or managed SFT, DPO, GRPO, KTO, RLOO, or reward-model training uses TRL.                                          |
| `train-sentence-transformers`       | `huggingface/skills`                  | Dense, sparse, reranker, or ColBERT-style embedding training recurs.                                                    |
| `huggingface-community-evals`       | `huggingface/skills`                  | Local model evaluation with inspect-ai or lighteval recurs.                                                             |
| `transformers-js`                   | `huggingface/skills`                  | Transformers.js inference runs in browsers, Node.js, Bun, or Deno through WebGPU or WASM.                               |
| `instrumenting-with-mlflow-tracing` | `mlflow/skills`                       | MLflow tracing of an AI application recurs.                                                                             |
| `agent-evaluation`                  | `mlflow/skills`                       | An existing agent needs systematic MLflow datasets, scorers, and evaluation.                                            |
| `build-a-scorer`                    | `mlflow/skills`                       | Agent or RAG quality criteria need reliable MLflow scorers.                                                             |
| `fix-agent-issue`                   | `mlflow/skills`                       | An agent behavior change should be grounded in traces and preserved as regression tests.                                |
| `analyzing-mlflow-trace`            | `mlflow/skills`                       | A single failed or low-quality agent trace needs root-cause analysis.                                                   |
| `analyzing-mlflow-session`          | `mlflow/skills`                       | A multi-turn agent session needs trace-based analysis.                                                                  |
| `ort-build`                         | `microsoft/onnxruntime`               | Work inside ONNX Runtime repeatedly needs targeted native, CUDA, WebGPU, or wheel builds.                               |
| `ort-test`                          | `microsoft/onnxruntime`               | Work inside ONNX Runtime needs focused C++, Python, execution-provider, or kernel-path verification.                    |
| `onnx-opset-bump-checklist`         | `microsoft/onnxruntime`               | The ONNX Runtime repository updates its pinned ONNX opset and related generated artifacts.                              |

For CUDA kernels, GPU debugging, profiling, or scientific Python GPU acceleration, open [CUDA and GPU acceleration](../systems/cuda.md).

For model endpoints, local model servers, or serving benchmarks, open [model serving](serving.md).
