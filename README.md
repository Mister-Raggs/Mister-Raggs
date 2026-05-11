## Raghav Kachroo

Backend engineer focused on distributed systems and operational reliability, currently applying that lens to AI infrastructure.

At Amazon I worked on high-throughput ingestion pipelines and cross-region observability. Before that, I built streaming data systems at a fintech startup (Kafka, Airflow, Elasticsearch at scale). I'm currently at UCSD's Hao AI Lab, where I contribute to [**FastVideo**](https://github.com/hao-ai-lab/FastVideo) — most recently [building the initial agent skill stack](https://github.com/hao-ai-lab/FastVideo/commit/e3a5c6954f49bb48ab72455df5f2f03cdab913dd) for automated model porting, with ongoing work on inference optimization via torch.compile and kernel fusion.

**Projects worth looking at:**

[**log-triage-v2**](https://github.com/Mister-Raggs/log-triage-v2) — Go service that routes noisy log streams to an LLM for triage, replacing a legacy publish pipeline that had a one-hour delay. Added binary search indexing, AWS Step Functions orchestration, and an MCP interface on top of the inherited Timber base.

[**Flare**](https://github.com/Mister-Raggs/flare) — Observability layer for LLM pipelines: structured eval metrics, cost tracking, and latency profiling across model calls. Built to make LLM behavior debuggable the same way you'd instrument any distributed service.

**Writing:** [mister-raggs.github.io](https://mister-raggs.github.io)  
**LinkedIn:** [linkedin.com/in/raghavkachroo](https://linkedin.com/in/raghavkachroo)
