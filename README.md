# Awesome AI Engineering Stack [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

![Reviewed](https://img.shields.io/badge/reviewed-September%205%2C%202026-informational)

> Open-source infrastructure and developer tooling for building, evaluating, deploying and operating modern AI systems.

A selective list spanning agents, retrieval, data, training, serving, evaluation, safety and production operations. Core entries are chosen for relevance, maintenance, licensing, adoption or stewardship, and distinct engineering utility; narrower ecosystems and lower-confidence projects live in companion indexes.

See [Curation](CURATION.md) for the evidence standard and [Notable exclusions](EXCLUSIONS.md) for deliberate omissions.

## Contents

- [Model Context Protocol](#model-context-protocol)
- [Agents and Orchestration](#agents-and-orchestration)
- [Coding Agents](#coding-agents)
- [Agent Memory](#agent-memory)
- [Browser and Computer Use](#browser-and-computer-use)
- [Structured Outputs and Constrained Generation](#structured-outputs-and-constrained-generation)
- [Retrieval, Vector Search and Knowledge](#retrieval-vector-search-and-knowledge)
- [Document Ingestion, OCR and Parsing](#document-ingestion-ocr-and-parsing)
- [Data and Dataset Engineering](#data-and-dataset-engineering)
- [Experiment Tracking and ML Lifecycle](#experiment-tracking-and-ml-lifecycle)
- [Training, Post-Training and Distributed Compute](#training-post-training-and-distributed-compute)
- [Inference and Serving](#inference-and-serving)
- [Gateways and Model Routing](#gateways-and-model-routing)
- [Evaluation and Benchmarks](#evaluation-and-benchmarks)
- [Safety, Red Teaming and Governance](#safety-red-teaming-and-governance)
- [Observability and Tracing](#observability-and-tracing)

## Model Context Protocol

*Canonical protocol resources and the production-grade SDK/debugging surface; the wider SDK and integration ecosystem is split out.*

- [Model Context Protocol](https://github.com/modelcontextprotocol/modelcontextprotocol) - Official MCP specification and documentation; the canonical source for protocol behavior and versioning.
- [MCP TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk) - Official TypeScript SDK for building MCP clients and servers.
- [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk) - Official Python SDK for building MCP clients and servers.
- [MCP C# SDK](https://github.com/modelcontextprotocol/csharp-sdk) - Official C# SDK for .NET MCP clients and servers.
- [MCP Go SDK](https://github.com/modelcontextprotocol/go-sdk) - Official Go SDK for MCP clients and servers.
- [MCP Inspector](https://github.com/modelcontextprotocol/inspector) - Official browser and CLI debugging tool for inspecting MCP servers, tools, resources and protocol traffic.
- [MCP Registry](https://github.com/modelcontextprotocol/registry) - Official registry and discovery service for MCP servers.

## Agents and Orchestration

*Reusable frameworks for state, tools, workflows and multi-agent coordination—not finished assistant applications.*

- [LangGraph](https://github.com/langchain-ai/langgraph) - Stateful orchestration framework for long-running and tool-using agents.
- [Pydantic AI](https://github.com/pydantic/pydantic-ai) - Typed Python framework for production-oriented agents and tool calling.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - Lightweight Python SDK for agents, handoffs, guardrails and tracing.
- [smolagents](https://github.com/huggingface/smolagents) - Lightweight Hugging Face agent framework for tool-calling and code-agent workflows.
- [CrewAI](https://github.com/crewAIInc/crewAI) - Role-oriented multi-agent orchestration framework with a large ecosystem.
- [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) - Microsoft framework for building tool-using and multi-agent applications with structured orchestration primitives.
- [DSPy](https://github.com/stanfordnlp/dspy) - Programmatic framework for optimizing LM pipelines, modules and prompts.
- [LangChain](https://github.com/langchain-ai/langchain) - General framework and integration ecosystem for LLM applications.
- [LlamaIndex](https://github.com/run-llama/llama_index) - Data, retrieval and agent framework for context-aware applications.
- [Haystack](https://github.com/deepset-ai/haystack) - Open framework for RAG pipelines, agents and production search applications.
- [Langroid](https://github.com/langroid/langroid) - MIT multi-agent framework with explicit message-passing abstractions.

## Coding Agents

*Open coding harnesses that can inspect repositories, edit files and execute development workflows.*

- [OpenHands](https://github.com/OpenHands/openhands) - Open software-development agent platform; the core is MIT, while enterprise code has separate terms.
- [Aider](https://github.com/Aider-AI/aider) - Terminal-based AI pair programmer with repository mapping, edits and test loops.
- [Cline](https://github.com/cline/cline) - Open coding agent for IDE and CLI workflows with repository editing, terminal execution and tool use.
- [OpenCode](https://github.com/anomalyco/opencode) - Open-source coding agent with terminal and desktop workflows, built-in agents and broad model-provider support.
- [Pi](https://github.com/earendil-works/pi) - Agent harness with a unified LLM API, stateful runtime and self-extensible coding-agent CLI.
- [Goose](https://github.com/aaif-goose/goose) - Extensible local coding agent with desktop and CLI interfaces plus MCP-based extensions.
- [Letta Code](https://github.com/letta-ai/letta-code) - Memory-first coding-agent harness for long-lived state across repository work.

## Agent Memory

*Reusable state and memory infrastructure for long-lived agents.*

- [Mem0](https://github.com/mem0ai/mem0) - Memory layer for agents and assistants; distinguish the Apache-2.0 core from managed-service features.
- [Letta Agent SDK](https://github.com/letta-ai/letta-agent-sdk) - SDK for building stateful Letta agents across local and hosted deployments.
- [Graphiti](https://github.com/getzep/graphiti) - Temporal knowledge-graph framework for agent memory and continuously changing facts.

## Browser and Computer Use

*Tooling for agents that operate browsers or interactive computer environments.*

- [Browser Use](https://github.com/browser-use/browser-use) - Framework for browser agents that can navigate, interact with and extract data from the web.
- [Stagehand](https://github.com/browserbase/stagehand) - Browser automation SDK that combines deterministic primitives with AI-powered actions, extraction and agents.

## Structured Outputs and Constrained Generation

*Libraries that make model output reliably conform to schemas, grammars or programmatic constraints.*

- [Instructor](https://github.com/567-labs/instructor) - Pydantic-based structured extraction, validation and retry layer across multiple LLM providers.
- [Outlines](https://github.com/dottxt-ai/outlines) - Constrained-generation library for schema-, type-, regex- and grammar-controlled structured outputs.
- [Guidance](https://github.com/guidance-ai/guidance) - Programming model for constrained and interleaved LLM generation using regex, grammars and control flow.

## Retrieval, Vector Search and Knowledge

*Core embedding, vector-search and knowledge infrastructure for RAG and agent memory.*

- [Qdrant](https://github.com/qdrant/qdrant) - Production vector database and search engine for dense, sparse, hybrid and multi-vector retrieval.
- [pgvector](https://github.com/pgvector/pgvector) - Vector similarity search extension for PostgreSQL with exact and approximate nearest-neighbor indexes.
- [Milvus](https://github.com/milvus-io/milvus) - Distributed vector database for large-scale similarity search and retrieval workloads.
- [Weaviate](https://github.com/weaviate/weaviate) - Open-source vector database with hybrid search, filtering and production deployment support.
- [Chroma](https://github.com/chroma-core/chroma) - AI-oriented search infrastructure for embedding retrieval and application memory.
- [LanceDB](https://github.com/lancedb/lancedb) - Vector database built on the Lance columnar format for local, embedded and production retrieval workflows.
- [FAISS](https://github.com/facebookresearch/faiss) - High-performance library for dense-vector similarity search and clustering on CPU and GPU.
- [Sentence Transformers](https://github.com/huggingface/sentence-transformers) - Dense, sparse and multi-vector embeddings plus reranking models.
- [FastEmbed](https://github.com/qdrant/fastembed) - Lightweight CPU-first embedding and reranking library; model licenses vary.
- [Neo4j](https://github.com/neo4j/neo4j) - Graph database frequently used for knowledge graphs and GraphRAG; Community Edition is GPL.

## Document Ingestion, OCR and Parsing

*High-signal tools for turning real documents into structured, searchable data; low-level primitives live in a specialist index.*

- [Docling](https://github.com/docling-project/docling) - Local document conversion and structured extraction for RAG and data pipelines.
- [Unstructured](https://github.com/Unstructured-IO/unstructured) - General document preprocessing and partitioning toolkit.
- [PyMuPDF](https://github.com/pymupdf/PyMuPDF) - High-performance PDF extraction and manipulation library; AGPL-3.0 or commercial licensing.
- [MarkItDown](https://github.com/microsoft/markitdown) - Microsoft MIT converter for turning common document formats into Markdown.
- [Xberg](https://github.com/xberg-io/xberg) - Rust-core document intelligence toolkit for extracting text, metadata, images, tables and structured data across many file formats.
- [OCRmyPDF](https://github.com/ocrmypdf/OCRmyPDF) - Mature OCR pipeline that adds searchable text layers to scanned PDFs.
- [Tesseract](https://github.com/tesseract-ocr/tesseract) - Foundational CPU-friendly OCR engine for printed text.
- [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR) - Modern multilingual OCR and document-parsing toolkit.
- [GROBID](https://github.com/grobidOrg/grobid) - Scholarly-document parser for structure, metadata and citations.
- [Apache Tika](https://github.com/apache/tika) - Broad file-type detection and text/metadata extraction across 1,000+ formats.

## Data and Dataset Engineering

*AI-specific dataset loading, curation, annotation and local processing rather than a general data-engineering catalog.*

- [Hugging Face Datasets](https://github.com/huggingface/datasets) - Dataset loading, streaming, processing and sharing library used across model training and evaluation workflows.
- [NeMo Curator](https://github.com/NVIDIA-NeMo/Curator) - Scalable data-curation toolkit for filtering, deduplication and preprocessing of large foundation-model datasets.
- [Label Studio](https://github.com/HumanSignal/label-studio) - General-purpose data annotation platform for text, images, audio, video and multimodal ML workflows.
- [DataTrove](https://github.com/huggingface/datatrove) - Composable large-scale data-processing pipelines for preparing training corpora and other model datasets.
- [dlt](https://github.com/dlt-hub/dlt) - Python data-ingestion library; distinguish the Apache-2.0 library from commercial dltHub services.
- [DuckDB](https://github.com/duckdb/duckdb) - Embedded analytical database for local data processing and pipelines.
- [Polars](https://github.com/pola-rs/polars) - High-performance DataFrame and query engine for single-node processing.
- [Apache Arrow](https://github.com/apache/arrow) - Foundational in-memory columnar format and multi-language data toolkit.

## Experiment Tracking and ML Lifecycle

*Reproducibility, artifacts, experiments and production workflow orchestration across the model lifecycle.*

- [MLflow](https://github.com/mlflow/mlflow) - MLOps platform with GenAI tracing, evaluation and experiment management.
- [DVC](https://github.com/treeverse/dvc) - Data and experiment versioning for reproducible ML workflows; linked to the canonical repository after the project move.
- [ZenML](https://github.com/zenml-io/zenml) - Open-source AI orchestration platform for reproducible pipelines, artifacts and production workflows.
- [Metaflow](https://github.com/Netflix/metaflow) - Python framework for developing and operating end-to-end AI/ML workflows from local iteration to production compute.
- [Flyte](https://github.com/flyteorg/flyte) - Kubernetes-native orchestration platform for resilient data, model and AI workflows at scale.

## Training, Post-Training and Distributed Compute

*Foundational frameworks and high-leverage tooling for training, fine-tuning, alignment and scaling compute.*

- [PyTorch](https://github.com/pytorch/pytorch) - Foundational tensor and deep-learning framework with strong GPU acceleration and a broad production ecosystem.
- [Transformers](https://github.com/huggingface/transformers) - Core model library and ecosystem for transformer-based models.
- [PEFT](https://github.com/huggingface/peft) - Parameter-efficient fine-tuning methods for large models.
- [Accelerate](https://github.com/huggingface/accelerate) - Hugging Face launcher and runtime layer for portable PyTorch training across devices, mixed precision, FSDP and DeepSpeed.
- [TRL](https://github.com/huggingface/trl) - Hugging Face post-training library for SFT, GRPO, DPO and related alignment workflows.
- [TorchAO](https://github.com/pytorch/ao) - PyTorch-native model optimization toolkit for quantization and low-precision training-to-serving workflows.
- [TorchTitan](https://github.com/pytorch/torchtitan) - PyTorch-native platform for large-scale model training.
- [DeepSpeed](https://github.com/deepspeedai/DeepSpeed) - Distributed training and optimization system for large models.
- [Megatron-LM](https://github.com/NVIDIA/Megatron-LM) - NVIDIA framework for large-scale transformer training.
- [NeMo AutoModel](https://github.com/NVIDIA-NeMo/Automodel) - NVIDIA-NeMo training component for building and fine-tuning modern model families.
- [NeMo RL](https://github.com/NVIDIA-NeMo/RL) - NVIDIA reinforcement-learning and post-training stack.
- [Megatron Bridge](https://github.com/NVIDIA-NeMo/Megatron-Bridge) - Bridge between Megatron training stacks and Hugging Face model ecosystems.
- [OpenRLHF](https://github.com/OpenRLHF/OpenRLHF) - RLHF and agentic-RL framework built around Ray and DeepSpeed.
- [verl](https://github.com/verl-project/verl) - Scalable post-training framework for reinforcement learning with LLMs.
- [TorchRL](https://github.com/pytorch/rl) - PyTorch reinforcement-learning library useful as a general RL foundation.
- [Unsloth](https://github.com/unslothai/unsloth) - Efficient fine-tuning toolkit with an Apache-2.0 core and AGPL-3.0 optional Studio components.
- [Axolotl](https://github.com/axolotl-ai-cloud/axolotl) - Configuration-driven framework for fine-tuning and post-training language models.
- [LLaMA-Factory](https://github.com/hiyouga/LlamaFactory) - Broad fine-tuning toolkit supporting many model families and training methods.
- [Ray](https://github.com/ray-project/ray) - Distributed AI compute engine for scaling training, data processing, reinforcement learning and model serving.

## Inference and Serving

*Runtimes and deployment layers for local, GPU, cluster and Kubernetes model serving.*

- [vLLM](https://github.com/vllm-project/vllm) - High-throughput LLM inference and OpenAI-compatible serving engine.
- [SGLang](https://github.com/sgl-project/sglang) - High-performance serving runtime for language and vision-language models.
- [llama.cpp](https://github.com/ggml-org/llama.cpp) - Portable local inference engine for GGUF models across CPU and GPU backends.
- [Ollama](https://github.com/ollama/ollama) - User-friendly local model runner and management layer.
- [TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) - NVIDIA-optimized LLM inference stack for high-performance GPU serving.
- [LMDeploy](https://github.com/InternLM/lmdeploy) - High-performance serving and inference toolkit for LLMs and VLMs.
- [BentoML](https://github.com/bentoml/BentoML) - Model and AI-application serving framework for production APIs.
- [KServe](https://github.com/kserve/kserve) - Kubernetes-native platform for scalable generative and predictive model inference.
- [Triton Inference Server](https://github.com/triton-inference-server/server) - Production inference server supporting multiple ML frameworks.
- [GPUStack](https://github.com/gpustack/gpustack) - Open multi-cluster GPU and model-serving management layer.
- [SkyPilot](https://github.com/skypilot-org/skypilot) - Cloud and cluster orchestration layer for AI compute workloads.

## Gateways and Model Routing

*Provider-neutral API gateways for routing, fallback, rate control and policy enforcement.*

- [LiteLLM](https://github.com/BerriAI/litellm) - OpenAI-compatible gateway and client layer with an MIT core and separately licensed enterprise functionality.
- [Envoy AI Gateway](https://github.com/envoyproxy/ai-gateway) - Open-source AI gateway built on Envoy Gateway for provider routing, authentication and rate limiting.
- [Bifrost](https://github.com/maximhq/bifrost) - Apache-2.0 OpenAI-compatible AI gateway with multi-provider routing, failover, load balancing and caching.
- [Portkey Gateway](https://github.com/Portkey-AI/gateway) - Open-source AI gateway for multi-provider routing, policy controls and guardrail integration.

## Evaluation and Benchmarks

*Frameworks for repeatable model, RAG and agent evaluation rather than benchmark leaderboards alone.*

- [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) - UK AI Security Institute framework for model and agent evaluations.
- [Inspect Evals](https://github.com/UKGovernmentBEIS/inspect_evals) - Community evaluation catalog built for Inspect AI.
- [Harbor](https://github.com/harbor-framework/harbor) - Containerized agent-evaluation and RL environment harness, including Terminal-Bench workflows.
- [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) - Widely used framework for standardized language-model evaluation.
- [Lighteval](https://github.com/huggingface/lighteval) - Hugging Face evaluation toolkit for models and training workflows.
- [HELM](https://github.com/stanford-crfm/helm) - Stanford framework for transparent, reproducible model evaluation.
- [OpenCompass](https://github.com/open-compass/opencompass) - Distributed evaluation platform supporting many models and benchmark suites.
- [DeepEval](https://github.com/confident-ai/deepeval) - LLM evaluation framework for tests, metrics and CI workflows.
- [Giskard](https://github.com/Giskard-AI/giskard-oss) - Open testing and evaluation framework for LLM and agent systems.

## Safety, Red Teaming and Governance

*Testing and runtime controls for adversarial evaluation, policy enforcement and agent governance.*

- [promptfoo](https://github.com/promptfoo/promptfoo) - Declarative testing, red teaming and CI for prompts, agents and RAG systems.
- [garak](https://github.com/NVIDIA/garak) - NVIDIA toolkit for probing and red teaming generative models.
- [PyRIT](https://github.com/microsoft/pyrit) - Microsoft AI Red Team framework for orchestrated adversarial testing.
- [NeMo Guardrails](https://github.com/NVIDIA-NeMo/Guardrails) - NVIDIA toolkit for programmable safety, dialog, retrieval and tool-use guardrails in LLM applications.
- [Agent Governance Toolkit](https://github.com/microsoft/agent-governance-toolkit) - Microsoft runtime governance toolkit for agent policies, controls and auditability.
- [Guardrails](https://github.com/guardrails-ai/guardrails) - Validation and guardrail framework for structured and policy-constrained LLM outputs.

## Observability and Tracing

*Tracing, telemetry and production monitoring for model and agent applications; experiment lifecycle is kept separate.*

- [Langfuse](https://github.com/langfuse/langfuse) - LLM tracing, evaluation, datasets and prompt-management platform with an MIT core and separately licensed enterprise directories.
- [Opik](https://github.com/comet-ml/opik) - Open LLM observability, evaluation and experiment platform.
- [OpenLLMetry](https://github.com/traceloop/openllmetry) - OpenTelemetry instrumentation for LLM and agent applications.
- [OpenLIT](https://github.com/openlit/openlit) - OpenTelemetry-native observability and evaluation stack for AI applications.
- [Evidently](https://github.com/evidentlyai/evidently) - Evaluation and monitoring for ML, LLM and data-quality workflows.

## Related indexes

- [MCP Ecosystem](MCP_ECOSYSTEM.md) - Additional official SDKs plus domain-specific MCP servers and integrations.
- [Document AI](DOCUMENT_AI.md) - Lower-level PDF, OCR, table-extraction and document-evaluation tooling.
- [AI Data Infrastructure](DATA_INFRASTRUCTURE.md) - Broader analytical engines, lakehouse formats and data foundations that are useful around AI workloads but too generic for the core list.
- [Watchlist](WATCHLIST.md) - Promising, young, adjacent or currently lower-confidence projects that are being tracked outside the core.
- [Notable exclusions](EXCLUSIONS.md) - Selected well-known projects intentionally left out, with the reason.

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md) before proposing an addition. A pull request should explain why a project deserves limited core-list space, not merely why the project exists.

