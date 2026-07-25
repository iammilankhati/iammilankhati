# Milan Khati
### Distributed Systems & Agentic AI Architect

I build high-throughput, fault-tolerant distributed backends and autonomous multi-agent systems. My focus is on long-running durable workflows, event-driven state orchestration, and highly optimized vector data pipelines.

- 🛠️ **Languages:** Python (AI/Data Logic), Go & Rust (High-Performance Proxies, Tooling, Core Infra)
- ⚙️ **Infrastructure:** Temporal, Kafka, Kubernetes, gRPC, Docker, OpenTelemetry
- 🤖 **Agentic & Vector:** LangGraph, Model Context Protocol (MCP), Custom State Machines, Qdrant, Redis

---

## Flagship Systems Architectural Focus

### 🐍 [agentic-mesh-orchestrator](https://github.com)
A durable, self-healing multi-agent orchestration runtime built for production.
- Implements state-machine transitions using **Temporal** to survive node crashes mid-agent-loop.
- Features secure tool execution sandboxing alongside Model Context Protocol (MCP) tool integration.

### 🐹 [ai-gateway-proxy-evaluator](https://github.com)
A low-latency, high-performance LLM gateway and continuous evaluation proxy written in Go.
- Built-in token streaming optimization, semantic caching sharding via **Redis**, and distributed rate-limiting.
- Streams real-time continuous evaluation performance metrics (LLM-as-a-judge) natively over **gRPC**.

### 🦀 [distributed-rag-ingestion-pipeline](https://github.com)
A horizontally scalable streaming data ingestion pipeline processing multi-modal documents into vector spaces.
- Real-time stream processing using **Kafka** and **Apache Flink** for distributed embedding generation.
- Implements multi-threaded text chunking algorithms and sliding token windows natively in Rust.
