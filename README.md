# Milan Khati
### Distributed Systems & Agentic AI Architect | Go • Rust • Python

I build high-throughput, fault-tolerant distributed backends and autonomous multi-agent systems. My focus is on long-running durable workflows, event-driven state orchestration, and highly optimized vector data pipelines.

- **Languages:** Python (AI/Data), Go & Rust (High-Performance Proxies, Tooling, Core Infra)
- **Infrastructure:** Temporal, Kafka, Kubernetes, gRPC, Docker, OpenTelemetry
- **Agentic & Vector:** LangGraph, CrewAI, Custom State Machines, Qdrant, Milvus

---

## Flagship Systems Architectural Focus

### [1] agentic-mesh-orchestrator (Python)
A durable, self-healing multi-agent orchestration runtime built for production. 
- Implements state-machine transitions using **Temporal** to survive node crashes mid-agent-loop.
- Features execution sandboxing for untrusted code execution and tool-calling.

### [2] ai-gateway-proxy-evaluator (Go)
A low-latency, high-performance LLM gateway and continuous evaluation proxy.
- Built-in token streaming optimization, semantic caching via **Redis**, and distributed rate-limiting.
- Real-time continuous evaluation (LLM-as-a-judge) streaming metrics over **gRPC**.

### [3] distributed-rag-ingestion-pipeline (Rust / Python)
A horizontally scalable data ingestion pipeline processing multi-modal documents into vector spaces.
- Real-time stream processing using **Kafka** for distributed embedding generation.
- Custom hybrid-search routing optimized for **Qdrant** clusters.
