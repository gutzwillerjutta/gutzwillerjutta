# Platform engineer focused on distributed ingestion and operational reliability.
## @gutzwillerjutta
I build durable APIs, queues, workers, and data pipelines that move records through multiple boundaries. I own failure modes in schemas, retries, caches, indexes, traces, and deployments. I prefer boring operational paths with explicit ownership, even when the implementation is less elegant. I accept duplicated normalization when it reduces downstream ambiguity.
### 🛠 Tech & Infrastructure
- **Core:** TypeScript, Fastify, gRPC
- **Data:** PostgreSQL, Redis, ClickHouse, Apache Kafka
- **Infra:** Docker, Kubernetes, Terraform
- **Tooling:** npm, OpenTelemetry, GitHub Actions
### ⚙️ Engineering Areas
- Backpressure-aware ingestion pipelines with idempotent workers.
- Schema evolution across Kafka topics, RPCs, and PostgreSQL migrations.
- Query indexes and cache invalidation for high-cardinality event data.
- Distributed tracing across APIs, queues, and deployment boundaries.
### 🔭 Current Focus
- Moving batch reconciliation into bounded workers without adding another queue.
- Reducing cache stale reads while preserving throughput under dependency latency.
- Testing Kafka schema migrations with consumers that support older wire formats.
- Shortening trace span creation without obscuring worker failure boundaries.
### 📌 Engineering Notes
- Retry only operations with an idempotency key or a durable replay path.
- Treat schema boundaries as contracts and keep validation close to ingestion.
- A migration should be observable before it is considered safe to remove.
- Error handling belongs at the queue boundary, not only inside request handlers.
### 🧭 How I Work
- I choose systems with observable failure modes over systems with fewer components.
- I keep operational changes separate from schema and API changes when rollback matters.

_I make the boring path reliable enough that novelty is optional._

[Email](mailto:gutzwillerjutta@gmail.com)