# ToDo: Refactoring AI Meal Coach Project for GitHub Repository

This ToDo list outlines the main tasks and a step-by-step guide for adapting and improving the AI Meal Coach project for local operation and a modular GitHub version.

---

## 📅 Phase 1: Set up basic structure

- [x] Create new repository: [Done]
- [x] Write initial README.md: [Done]
- [ ] Create base folders (`model/`, `utils/`, `data/`, `examples/`)
- [ ] Prepare `requirements.txt` (minimal set)
- [ ] Prepare `main.py` with a simple command-line loop (input + agent call)

---

## 📚 Phase 2: Replace Gemini API with Bielik model

- [ ] Research how to run Bielik model locally (HF Transformers / vLLM / llama.cpp)
- [ ] Create `model/load_bielik_model.py`
- [ ] Implement a function that generates responses from Bielik locally
- [ ] Replace all Gemini function calls with Bielik calls (in search/adapt/evaluate)

---

## 🔄 Phase 3: Rework recipe search and embedding logic

- [ ] Load FAISS index and metadata from local files
- [ ] Move search logic into `utils/search.py`
- [ ] Ensure queries are embedded with local embedding model or re-use pre-computed embeddings

---

## 📈 Phase 4: Improve tool functions

- [ ] Move recipe adaptation into `utils/adapt.py`
- [ ] Move dietary evaluation logic into `utils/evaluate.py`
- [ ] (Optional) Fine-tune prompts for Bielik if needed

---

## 🛋️ Phase 5: CLI (Command-Line Interface)

- [ ] Create a simple text-based conversation flow in `main.py`
- [ ] Allow user to:
  - [ ] Specify ingredients
  - [ ] Choose a diet profile
  - [ ] Ask to adapt a recipe
  - [ ] Check if a recipe fits a diet

---

## 👾 Future Ideas (Optional Extensions)

- [ ] Add a simple web UI using Streamlit or Gradio
- [ ] Add error handling and better prompts
- [ ] Save conversation history to file (optional)
- [ ] Dockerize the project for easier deployment

---

# Let's build a local, privacy-first AI meal assistant! 🚀
