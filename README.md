## Raghav Kachroo

Software engineer focused on distributed systems and operational reliability, currently applying that lens to AI infrastructure.

At Amazon I worked on high-throughput log indexing and on-call automation. Before that, I built document intelligence systems at Aark Global — async ingestion pipelines, OCR, search, and datastore migration — and earlier, streaming data infrastructure at Concentrix (Kafka, Airflow, Elasticsearch at scale). I'm currently at UCSD's Hao AI Lab, contributing to [**FastVideo**](https://github.com/hao-ai-lab/FastVideo), an open-source video-diffusion framework. Recent shipped work: [a PostDecode optimization](https://github.com/hao-ai-lab/FastVideo/pull/1362) that cut Cosmos 2.5 end-to-end latency by **15.6%** (cross-validated on H100), [torch.compile documentation](https://github.com/hao-ai-lab/FastVideo/pull/1366) surfacing a hidden **24%** speedup, [the Cosmos 2.5 training pipeline](https://github.com/hao-ai-lab/FastVideo/pull/1227) (LoRA + full fine-tune, merged), and [FA2/FA3 as a torch.library custom_op](https://github.com/hao-ai-lab/FastVideo/pull/1373) — the traceable-node enabler for downstream graph-break work. Current focus: real backward registration for FlashAttention under `torch.compile` and the broader inference-optimization loop.

**Projects worth looking at:**

[**log-triage-v2**](https://github.com/Mister-Raggs/log-triage-v2) — Go log indexing engine, a portable rewrite of an internal Amazon tool. Time-sorted index with binary search (49ns at 1k entries, 77ns at 1M — cache-dominated, not comparison-bound), channel-based worker pool for parallel ingestion at 42M rows/hour, write-ahead log with batched fsync, Prometheus + OpenTelemetry instrumentation.

[**Flare**](https://github.com/Mister-Raggs/flare) — End-to-end ML log anomaly detection pipeline. Drain3 template mining + multi-model scoring (Isolation Forest, LOF, One-Class SVM) + DBSCAN incident clustering + Claude summarization. 0.642 F1 at ~40ms CPU-only latency on the full HDFS dataset (11.2M lines), LLM-as-judge eval scoring 4.67/5 without ground truth labels, MLflow experiment tracking across runs.

**Writing:** [mister-raggs.github.io](https://mister-raggs.github.io)  
**LinkedIn:** [linkedin.com/in/raghavkachroo](https://linkedin.com/in/raghavkachroo)
