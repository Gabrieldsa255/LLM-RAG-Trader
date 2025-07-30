# LLM-RAG-Trader
LLM model for trade

<!-- Banner ------------------------------------------------------------ -->
<h1 align="center">🚀 rag-llama-quant</h1>
<p align="center">
  <strong>LLM-powered trading notebook</strong> that turns raw PDF playbooks and live market data<br>
  into actionable <em>buy/sell</em> signals on the 5-minute chart.
</p>

<p align="center">
  <img src="docs/demo.gif" alt="Demo GIF" width="720">
</p>

<!-- Badges ------------------------------------------------------------ -->
<p align="center">
  <a href="https://github.com/<USER>/rag-llama-quant/actions">
    <img src="https://img.shields.io/github/actions/workflow/status/<USER>/rag-llama-quant/tests.yml?label=tests&logo=github" alt="Build Status">
  </a>
  <a href="https://github.com/<USER>/rag-llama-quant/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/<USER>/rag-llama-quant?color=brightgreen" alt="License MIT">
  </a>
  <img src="https://img.shields.io/badge/python-3.10%20|%203.11-blue" alt="Python versions">
  <img src="https://img.shields.io/badge/model-Llama3-8B-GGUF-orange" alt="Model">
</p>

---

## ✨ Why this project?

Most open-source “AI traders” either  
1. show synthetic toy data or  
2. hide the logic behind paid APIs.

**rag-llama-quant** is fully reproducible, 100 % local (*Ollama* + *Chroma*), and teaches step-by-step how to:

* **Index** your own trading PDFs/notes with LangChain **RAG**  
* **Query** an LLM (*Llama 3 8B*) for cycle classification (channel → sideways → breakout)  
* **Fetch** real-time candles via `ccxt` and suggest precise *entry*, *stop* and *target*  
* Run everything in a clear Jupyter notebook you can tweak live.

---

## 🔥 Demo

> _“Show, don’t tell.”_  
> Clone → install → run cell ▸ see signals appear in ~30 s.

```bash
git clone https://github.com/<USER>/rag-llama-quant.git
cd rag-llama-quant
python -m venv venv && source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
jupyter lab LLM_Trader_M5.ipynb
