# Fireducks_Vs_Spark
# FireDucks vs Spark: Benchmarking Big Data Tools

![FireDucks vs Spark Benchmark Comparison](https://img.shields.io/badge/benchmark-results-brightgreen) 
![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

This repository contains benchmark tests comparing the performance of **FireDucks** (a high-performance single-machine engine) and **Apache Spark** (distributed processing) for different data analytics workloads.

## 🔥 Key Findings

| Metric               | FireDucks (10GB) | Spark (10GB) | Spark (100GB) |
|----------------------|------------------|--------------|---------------|
| **Read Time**        | 2s               | 15s          | 25s           |
| **GroupBy Time**     | 5s               | 20s          | 35s           |
| **Memory Usage**     | 1.2GB            | 3GB          | 8GB/node      |
| **Setup Overhead**   | None             | 20s          | 20s           |

**Conclusion**: FireDucks outperforms Spark on single-machine workloads, while Spark scales better for distributed data.

## 🛠️ Setup

1. Clone the repo:
```bash
git clone https://github.com/Agnivaghoshroy/Fireducks_Vs_Spark.git
cd Fireducks_Vs_Spark
