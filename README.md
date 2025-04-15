# 🚀 FireDucks vs. Spark: The Big Data Benchmarking Project

---

## 📌 Purpose
This project compares **FireDucks** (a high-performance single-machine engine) against **Spark** (distributed processing) to answer:

---

## 🛠️ Tech Stack

### 🔥 FireDucks Stack
| Component       | Technology           | Purpose                          |
|----------------|---------------------|----------------------------------|
| Core Engine    | DuckDB              | Single-machine OLAP queries      |
| Memory Mgmt    | Arrow               | Zero-copy data processing        |
| Optimizations  | Vectorized Execution | CPU-efficient operations         |

### ⚡ Spark Stack
| Component       | Technology           | Purpose                          |
|----------------|---------------------|----------------------------------|
| Core Engine    | Apache Spark 3.5    | Distributed data processing      |
| Cluster Mgmt   | YARN                | Resource allocation             |
| SQL Engine     | Catalyst            | Query optimization              |

---

## 🔥 Key Insights at a Glance

<div align="center">

| Metric               | FireDucks (10GB) | Spark (10GB) | Winner          |
|----------------------|------------------|--------------|-----------------|
| ⏱️ **Read Time**     | 2s               | 15s          | 🏆 FireDucks    |
| 🧮 **GroupBy Time**  | 5s               | 20s          | 🏆 FireDucks    |
| 💾 **Memory Usage**  | 1.2GB            | 3GB          | 🏆 FireDucks    |
| 🏗️ **Setup Time**   | Instant          | 20s          | 🏆 FireDucks    |
| 🌐 **Max Data Size** | ~50GB            | Unlimited    | 🏆 Spark        |

</div>

> **💡 Pro Tip**: FireDucks delivers **5-10x faster performance** on single-machine workloads, while Spark dominates at petabyte scale.

---

## 📖 Blog Post

Read the full blog here:
https://docs.google.com/document/d/1EQmkEs458scQnfgqVZHMNocOwww_XoKUQOQEqSqah8M/edit?usp=sharing

---

## 🧪 Colab Notebook
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://docs.google.com/document/d/1EQmkEs458scQnfgqVZHMNocOwww_XoKUQOQEqSqah8M/edit?usp=sharing)

Fully reproducible benchmark environment featuring:
```python
# Sample Colab Cell
!pip install fireducks spark
import fireducks as fd
