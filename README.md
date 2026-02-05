# 👋 Hi, I'm Ty Kana (@Nagamiji)

### 🇰🇭 Building Production AI Systems for Khmer Language & Public Impact
> Data Scientist | AI Engineer | Open Source Contributor

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?logo=linkedin&logoColor=white)](https://linkedin.com/in/yourprofile)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?logo=vercel&logoColor=white)](https://portfolio-ecru-alpha-16.vercel.app/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?logo=gmail&logoColor=white)](mailto:kanaty0153@gmail.com)

---

## 🚀 Why My Code Stands Out

I don't just build models — I ship **production-ready AI systems** with attention to:

✅ **MLOps rigor**: Dockerized environments, async processing, comprehensive logging  
✅ **Low-resource optimization**: 96% accuracy on Khmer digit recognition with efficient architectures (LSTM/GRU)  
✅ **Vector search expertise**: pgvector + OpenAI embeddings for semantic retrieval (10× faster queries)  
✅ **Full-stack ownership**: From data collection (Streamlit UIs) → model training → FastAPI deployment  

> *"My Khmer digit recognition system processes 15K+ handwritten samples — built entirely in Cambodia, for Cambodia."*

---

## 📦 Featured Repositories (Pinned)

### 🔬 Khmer NLP/CV Research
| Repo | What It Proves | Tech Stack |
|------|----------------|------------|
| [`khmer_stopword_removal_system`](https://github.com/Nagamiji/khmer_stopword_removal_system) | Production-ready NLP pipeline for low-resource Khmer language | Python, Regex, Unicode normalization |
| [`article_classifier`](https://github.com/Nagamiji/article_classifier) | Embedding-based classification with custom preprocessing | Transformers, scikit-learn, FastAPI |
| *Coming soon* | Khmer digit recognition dataset + LSTM/GRU models | PyTorch, Streamlit, Attention mechanisms |

### 🤖 Production AI Systems
| Repo | What It Proves | Tech Stack |
|------|----------------|------------|
| [`Edumind`](https://github.com/Nagamiji/Edumind) | End-to-end RAG chatbot with pgvector + Ollama | FastAPI, PostgreSQL/pgvector, MongoDB |
| [`Diagnosis-Disease`](https://github.com/Nagamiji/Diagnosis-Disease) | Healthcare ML with Flask API + treatment recommendation engine | scikit-learn, Flask, Pandas |
| [`EcommerceBackend`](https://github.com/Nagamiji/EcommerceBackend) | Scalable Spring Boot microservice with JWT auth | Java, Spring Boot, MySQL, Docker |

---

## 💡 Engineering Highlights (From My Repos)

### 📊 Spectrum Pricing Model (MoTP Project)
```python
# Ridge regression achieved 92% accuracy on 100K+ records
from sklearn.linear_model import RidgeCV
model = RidgeCV(alphas=np.logspace(-3, 3, 100), cv=5)
model.fit(X_train_scaled, y_train)
print(f"R² Score: {model.score(X_test_scaled, y_test):.3f}")  # 0.921
```
✅ Clean EDA notebooks with Pandas profiling  
✅ Feature engineering documented in `FEATURES.md`  
✅ Model comparison table (Linear/Ridge/Lasso/RF/SVR)

### ⚡ pgvector Optimization (Scholarar Internship)
```sql
-- Before: 200ms query latency
CREATE INDEX ON scholarships USING ivfflat (embedding vector_cosine_ops) 
WITH (lists = 100);

-- After: 20ms query latency (10× faster)
CREATE INDEX ON scholarships USING hnsw (embedding vector_cosine_ops);
```
✅ Docker Compose setup for pgvector isolation  
✅ Benchmark scripts comparing IVFFlat vs HNSW  
✅ OpenAPI spec for recommendation API

### 🖊️ Khmer Handwriting Data Pipeline
```python
# Streamlit UI capturing stroke coordinates in real-time
def capture_strokes(canvas):
    strokes = []
    for stroke in canvas.json_data["objects"]:
        points = [(p["x"], p["y"]) for p in stroke["path"]]
        strokes.append(points)
    return strokes  # → Saved as (x,y,t) sequences for LSTM training
```
✅ Unicode normalization for Khmer script (U+1780–U+17FF)  
✅ Data validation to reject incomplete characters  
✅ Dataset versioning with DVC

---

## 🛠️ Tech Stack Deep Dive

### AI/ML Engineering
![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/-TensorFlow-FF6F00?logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/-scikit--learn-F7931E?logo=scikit-learn&logoColor=white)
![Vertex AI](https://img.shields.io/badge/-Vertex_AI-4285F4?logo=google-cloud&logoColor=white)

### Vector Search & MLOps
![pgvector](https://img.shields.io/badge/-pgvector-4169E1?logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?logo=fastapi&logoColor=white)
![MLflow](https://img.shields.io/badge/-MLflow-000000?logo=mlflow&logoColor=white)

### Backend Engineering
![Java](https://img.shields.io/badge/-Java-007396?logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/-Spring_Boot-6DB33F?logo=spring&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?logo=postgresql&logoColor=white)

---

## 📊 GitHub Activity

![Kana's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Nagamiji&show_icons=true&theme=radical&count_private=true&include_all_commits=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Nagamiji&layout=compact&theme=radical&langs_count=8)

---

## 🤝 Let's Build Together

I'm actively seeking **Data Science / AI Engineer roles** where I can:
- Ship production ML systems with MLOps best practices
- Advance Khmer language AI (NLP/CV) for social impact
- Solve complex problems in public sector or startup environments

📧 **kanaty0153@gmail.com** | 🌐 **[Portfolio](https://portfolio-ecru-alpha-16.vercel.app/)** | 💼 **[LinkedIn](https://www.linkedin.com/in/kana-ty-3080a42aa/)**
