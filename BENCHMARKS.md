# VectorBench Vector Database Performance Benchmarks

Empirical QPS, Recall@10, and RAM consumption benchmarks across pgvector, Qdrant, Milvus, and Pinecone on 1M 1536-dim vectors.

⚡ **Explore VectorBench Leaderboard:** [https://vectorbench-hq.netlify.app/](https://vectorbench-hq.netlify.app/)

## 1. 1,000,000 Vectors (1536-dim OpenAI Embeddings)

| Engine & Index | Recall@10 | Queries Per Second (QPS) | RAM Footprint | Build Duration |
| :--- | :--- | :--- | :--- | :--- |
| Qdrant (HNSW m=16) | 99.2% | 1,450 QPS | 7.8 GB | 14 min |
| pgvector (HNSW m=16) | 98.4% | 890 QPS | 9.4 GB | 28 min |
| pgvector (IVFFlat lists=1000) | 91.0% | 310 QPS | 6.4 GB | 6 min |
| Milvus (HNSW) | 98.9% | 1,620 QPS | 8.2 GB | 18 min |

---
Maintained by [VectorBench](https://vectorbench-hq.netlify.app/).

## 📚 In-Depth Technical Implementation Guides

| Target Engineering Query | Production Reference & Guide URL |
| :--- | :--- |
| **Qdrant Vs Pinecone Benchmark** | [https://vectorbench-hq.netlify.app/qdrant-vs-pinecone-benchmark-2026/](https://vectorbench-hq.netlify.app/qdrant-vs-pinecone-benchmark-2026/) |
| **Pgvector Production Tuning Hnsw** | [https://vectorbench-hq.netlify.app/pgvector-production-tuning-guide/](https://vectorbench-hq.netlify.app/pgvector-production-tuning-guide/) |
| **Hnsw Vs Ivfflat Memory Consumption Pgvector** | [https://vectorbench-hq.netlify.app/hnsw-vs-ivfflat-pgvector/](https://vectorbench-hq.netlify.app/hnsw-vs-ivfflat-pgvector/) |
| **Cohere Embed V3 Vs Text-Embedding-3-Large Cost** | [https://vectorbench-hq.netlify.app/cohere-vs-openai-embeddings/](https://vectorbench-hq.netlify.app/cohere-vs-openai-embeddings/) |

