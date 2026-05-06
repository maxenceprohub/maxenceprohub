<div align="center">
  <h1>🌌 Zenith Engine</h1>
  <p><strong>Blazing-fast, memory-safe document intelligence for the AI era.</strong></p>

  [![Python 3.12+](https://img.shields.io/badge/Python-3.12%2B-blue.svg?style=for-the-badge&logo=python)](https://www.python.org)
  [![Rust Core](https://img.shields.io/badge/Rust-Powered-orange.svg?style=for-the-badge&logo=rust)](https://www.rust-lang.org)
  [![License: MIT](https://img.shields.io/badge/License-MIT-success.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
  [![Status](https://img.shields.io/badge/Status-Active_Development-purple.svg?style=for-the-badge)]()
</div>

<br>

> **Zenith Engine** bridges the gap between Python's AI flexibility and Rust's raw execution speed. It is designed to ingest, process, and index massive amounts of unstructured data with zero memory bottlenecks, making it the perfect foundation for local LLMs and RAG (Retrieval-Augmented Generation) pipelines.

---

## ✨ Enterprise-Grade Features

*   ⚡ **Hybrid Architecture:** High-level API written in Python, heavy-lifting memory management and parallel processing handled by Rust (`PyO3`).
*   🧠 **AI-Ready:** Seamless integration with OpenAI and Gemini endpoints for instant semantic analysis.
*   🛡️ **Fault Tolerant:** Bulletproof error handling for corrupted files, locked directories, and UTF-8 encoding failures.
*   📊 **Rich Terminal UI:** Real-time visual feedback, telemetry, and progress tracking using the `rich` library.

---

## ⚡ Performance Benchmark (Expected)

Zenith is built to outperform standard Python indexing scripts by offloading I/O and tokenization tasks.

| Task (10,000 files) | Standard Python | Zenith (Python + Rust) | Speedup |
| :--- | :--- | :--- | :--- |
| **Directory Scan** | 4.2s | **0.8s** | `5.2x` |
| **Text Extraction** | 18.5s | **3.1s** | `5.9x` |
| **Memory Peak** | 850 MB | **120 MB** | `-85%` |

---

## 🏗️ System Architecture
```text
zenith-engine/
├── 🦀 zenith_core/          # Rust library (Memory safe indexing & compression)
├── 🐍 zenith_api/           # Python wrapper (Logic, LLM connections)
├── 🖥️ cli.py                # Command Line Interface (Rich UI)
├── 📄 config.json           # User configurations
└── 🧪 tests/                # Automated testing suite
