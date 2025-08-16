# 🛍️ Comparing Recommender Systems: Cross-Filtering vs LLM-Based  

This project explores two distinct approaches to building recommender systems:  

1. **Cross-Filtering (Collaborative Filtering):**  
   A traditional recommender system that leverages user–item interaction data to identify patterns (e.g., “users who liked X also liked Y”).  

2. **LLM-Based Recommendations:**  
   A modern approach using **Large Language Models (LLMs)** to understand user intent and item descriptions in natural language, enabling **semantic, context-aware recommendations**.  

The goal is to **benchmark and compare** these two paradigms in terms of accuracy, F1 score, and qualitative recommendation quality.  

---

## 🚀 Systems Overview  

### 🔹 Cross-Filtering (Baseline)  
- Implements **user-based and item-based collaborative filtering**.  
- Relies on an **interaction matrix** (ratings, clicks, or purchases).  
- Strength: Learns from real user behavior.  
- Weakness: Struggles with **cold-start users/items**.  

### 🔹 LLM-Based Recommender  
- Uses a **Large Language Model** (via Hugging Face / OpenAI) to encode:  
  - **User queries** (e.g., “I want a lightweight laptop with strong battery life”).  
  - **Item metadata/descriptions** (e.g., product specs, reviews).  
- Matches embeddings to suggest semantically relevant items.  
- Strength: Handles **cold-starts** well and understands **nuanced preferences**.  
- Weakness: Requires **high-quality text data** and can be computationally expensive.  

---

## 📊 Performance Benchmarking  

We evaluate both systems on:  
- **F1 Score, Precision, Recall** → quantitative performance.  
- **Coverage & Diversity** → how varied and broad the recommendations are.  
- **Cold-Start Handling** → performance on new/unseen users or items.  

---

## 🛠️ Tech Stack  

- **Languages & Libraries:** Python, NumPy, Pandas, Scikit-learn  
- **Models:** Collaborative Filtering (baseline), Transformer-based LLMs (semantic)  
- **Tools:** Hugging Face (transformers), Streamlit (demo interface), PyTorch  

---

## 📂 Repository Structure  

