# AI Meal Coach: Health-Aware GenAI Meal Planner

This repository contains my Capstone Project developed during the **Gen AI Intensive Course with Google** on Kaggle (March-April 2025). Originally submitted as part of the Kaggle Capstone Competition, this project demonstrates how GenAI can support healthy meal planning based on dietary needs and available ingredients.

I am currently rebuilding the project for local use by:
- Refactoring the project into a modular Python package
- Moving from Gemini (cloud-based) to a **local LLM (Bielik)**
- Adding unit and integration tests using `pytest`
- Organizing the codebase into `src/` and `tests/` folders

---

## ✨ Project Overview

Planning healthy meals with dietary restrictions like **Hashimoto's**, **Type 2 Diabetes**, **Celiac Disease**, or **vegan diets** can be challenging and time-consuming. AI Meal Coach assists users by:

- Recommending recipes based on specific health profiles
- Searching a recipe database based on available fridge ingredients
- Adapting existing recipes to fit dietary restrictions (conceptually)
- Explaining whether a recipe meets health requirements

---

## 💻 Technology Stack

- **Model**: [Bielik]([https://hf.co/Polish-Bielik](https://huggingface.co/speakleash)) (local LLM),  previously Gemini API (Google)
- **Semantic Search**: FAISS for recipe retrieval (vector similarity search)
- **Embeddings**: Pre-generated or dynamically created
- **Python Libraries**: `transformers`, `faiss-cpu`, `numpy`, `pandas`, `pytest`
- **Environment**: Python 3.10+, virtualenv (`venv`), VSCode, GitHub Copilot

---

## 🗂️ Repository Structure (work in progress)

```
ai-meal-coach-bielik/
├── README.md
├── requirements.txt
├── .gitignore
├── .venv/ # Local virtual environment (excluded from repo)
├── src/ai_meal_coach/ # Main application code
│ ├── init.py
│ ├── main.py
│ ├── model/
│ │ └── load_bielik_model.py
│ ├── utils/
│ │ ├── search.py
│ │ ├── adapt.py
│ │ └── evaluate.py
│ └── data/
│ ├── recipes.csv
│ └── recipe_index.faiss
├── tests/ # Unit and integration tests
│ ├── init.py
│ ├── test_utils/
│ │ └── test_search.py
│ └── test_main.py
├── examples/
│ └── conversation_demo.txt
```

## 🧪 Running Tests

Tests are written using `pytest`. To run all tests:

```bash
pytest tests/

---

## 📎 Original Capstone Notebook

You can find the original submission on Kaggle:
https://www.kaggle.com/code/ankazieliska/ai-meal-coach-health-aware-ai-meal-planner

---

## 📈 Future Work

- Full integration with the Bielik model
- Complete RAG pipeline for diet + recipe search
- Streamlit or Gradio UI
- Extended health profiles and allergens support
- Improved search and matching logic

---

**#GenAI #LLM #AIForHealth #Python #CapstoneProject #LangChain #LangGraph #Hashimoto #Kaggle #Google #OpenToWork #AIProjects #WomenInTech #AIForGood**
