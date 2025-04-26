# AI Meal Coach: Health-Aware GenAI Meal Planner

This repository contains my Capstone Project developed during the **Gen AI Intensive Course with Google** on Kaggle (March-April 2025). Originally submitted as part of the Kaggle Capstone Competition, this project demonstrates how GenAI can support healthy meal planning based on dietary needs and available ingredients.

I am currently working on expanding and improving the project here by:
- Refactoring the project structure for better modularity
- Switching the main language model from a cloud-based Gemini API to a **local Bielik model** for fully offline operation

---

## ✨ Project Overview

Planning healthy meals with dietary restrictions like **Hashimoto's**, **Type 2 Diabetes**, **Celiac Disease**, or **vegan diets** can be challenging and time-consuming. AI Meal Coach assists users by:

- Recommending recipes based on specific health profiles
- Searching a recipe database based on available fridge ingredients
- Adapting existing recipes to fit dietary restrictions (conceptually)
- Explaining whether a recipe meets health requirements

---

## 💻 Technology Stack

- **Model**: [Bielik]([https://hf.co/Polish-Bielik](https://huggingface.co/speakleash)) (local LLM, in progress)
- **Semantic Search**: FAISS for recipe retrieval
- **Embeddings**: Pre-generated or custom embeddings
- **Python Libraries**: `transformers`, `faiss-cpu`, `numpy`, `pandas`

---

## 🗂️ Repository Structure (work in progress)

```
📁 ai-meal-coach-bielik/
├── README.md
├── requirements.txt
├── main.py
├── model/
│   └── load_bielik_model.py
├── data/
│   ├── recipes.csv
│   └── recipe_index.faiss
├── utils/
│   ├── search.py
│   ├── adapt.py
│   └── evaluate.py
└── examples/
    └── conversation_demo.txt
```

---

## 📎 Original Capstone Notebook

You can find the original submission on Kaggle:
https://www.kaggle.com/code/ankazieliska/ai-meal-coach-health-aware-ai-meal-planner

---

## 📈 Future Work

- Full integration with the Bielik model
- Full recipe adaptation pipeline
- Streamlit or Gradio UI
- Extended health profiles and allergens support
- Improved search and matching logic

---

**#GenAI #LLM #AIForHealth #Python #CapstoneProject #LangChain #LangGraph #Hashimoto #Kaggle #Google #OpenToWork #AIProjects #WomenInTech #AIForGood**
