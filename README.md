# SUMM AI 📄🤖

A Streamlit-powered research paper summarizer built with LangChain and Meta's **Llama 3.1 8B Instruct** model via HuggingFace. SUMM AI lets you generate tailored summaries of landmark AI research papers — customized by explanation style and length.

---

## Features

- 🧠 **LLM-powered summaries** using `meta-llama/Llama-3.1-8B-Instruct` via HuggingFace Inference API
- 📚 **Curated paper selection** covering foundational AI research
- 🎨 **Flexible explanation styles** — from beginner-friendly to mathematical
- 📏 **Adjustable summary length** — short, medium, or detailed
- ⚡ **Simple one-click interface** built with Streamlit

---

## Supported Research Papers

| Paper |
|-------|
| Attention Is All You Need |
| BERT: Pre-training of Deep Bidirectional Transformers |
| GPT-3: Language Models are Few-Shot Learners |
| Diffusion Models Beat GANs on Image Synthesis |

---

## Tech Stack

- [Streamlit](https://streamlit.io/) — UI framework
- [LangChain](https://www.langchain.com/) — Prompt management and LLM chaining
- [HuggingFace Inference API](https://huggingface.co/inference-api) — Model hosting
- [python-dotenv](https://pypi.org/project/python-dotenv/) — Environment variable management

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/summ-ai.git
cd summ-ai
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Set up your environment

Create a `.env` file in the project root and add your HuggingFace API token:

```env
HUGGINGFACEHUB_API_TOKEN=your_token_here
```

> Get your free token at [huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)

### 4. Run the app

```bash
streamlit run app.py
```

---

## Usage

1. Select a **research paper** from the dropdown
2. Choose an **explanation style** (Beginner-Friendly, Technical, Code-Oriented, or Mathematical)
3. Pick a **summary length** (Short, Medium, or Long)
4. Hit **Summarize** and let the model do the work

---

## Requirements
```
streamlit
langchain
langchain-huggingface
langchain-core
python-dotenv
```

---

## Project Structure
```
summ-ai/
├── app.py          # Main application
├── .env            # API keys (not committed)
├── .gitignore
├── requirements.txt
└── README.md
```
---

## Notes

- The model will respond with *"Insufficient information available"* rather than hallucinating details not present in the paper.
- Summaries include mathematical equations and analogies where relevant, based on your selected style.

---

## License

MIT License
