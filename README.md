# 🧑‍💻🤖 AI Codebase Understanding and Modernization Agent

🚀 A Python-based developer tool that indexes a code repository, searches for relevant code, summarizes module structure, and surfaces modernization suggestions.

## ✨ Features
- 📁 Repository scanning with generated folders excluded
- 🔎 Code search using TF-IDF and cosine similarity
- 🧩 Python classes, functions, and import analysis using AST
- 📝 Heuristic module summaries
- 🛡️ Potential risk-pattern flags for human review
- 🧪 Basic validation checks

## 🧰 Tech Stack
- 🐍 Python
- 📊 pandas
- 🧠 scikit-learn
- 🌳 Python AST
- 📓 Jupyter Notebook

## 🚀 Getting Started

Clone your repository:
```bash
git clone https://github.com/YOUR-USERNAME/ai-codebase-understanding-modernization-agent.git
cd ai-codebase-understanding-modernization-agent
```

Install dependencies:
```bash
pip install -r requirements.txt
jupyter notebook
```

Open `ai_codebase_understanding_modernization_agent.ipynb` and set `REPO_PATH` to the local repository you want to inspect.

## 🔄 Workflow
📁 Repository → 🧹 File Scanning → 🔎 Code Search → 🧩 Structure Analysis → 🛡️ Review Flags → 🧑‍💻 Human Review

## 💡 Use Cases
- Find authentication or validation logic
- Understand unfamiliar modules
- Explore classes, functions, and imports
- Find files relevant to refactoring
- Identify patterns that deserve manual security review

## ⚠️ Limitations
- TF-IDF is lexical search and can miss semantic matches.
- Deep structure analysis is currently focused on Python.
- Summaries are heuristic, not LLM-generated.
- Review flags may produce false positives or false negatives.
- This tool does not execute or modify code and is not a security guarantee.

## 🛣️ Roadmap
- [ ] 🧠 Add LLM explanations with file and line citations
- [ ] 🔎 Add embedding-based search and reranking
- [ ] 🗺️ Build a dependency graph
- [ ] 🛠️ Generate proposed code diffs for human approval
- [ ] 🧪 Add isolated test execution and regression checks
- [ ] 🔐 Add secret and dependency scanning
- [ ] 🌐 Build a FastAPI backend and interactive UI

## 🔒 Responsible Use
- 🚫 Never commit API keys or passwords.
- 📂 Treat repository files as untrusted input.
- 🧯 Do not execute unknown code just to analyze it.
- ✋ Review all suggestions and test changes before applying them.
- ☁️ Do not send proprietary source code to external services without permission.

## 📚 Learning Resources
- [Python AST](https://docs.python.org/3/library/ast.html)
- [scikit-learn text feature extraction](https://scikit-learn.org/stable/modules/feature_extraction.html#text-feature-extraction)
- [GitHub CodeQL](https://codeql.github.com/)
- [Semgrep](https://semgrep.dev/)

## 📄 License
Choose a license that matches your reuse goals. If you choose MIT, add a `LICENSE` file before claiming the project is MIT-licensed.

⭐ If you find this project useful, star the repository and share suggestions!
