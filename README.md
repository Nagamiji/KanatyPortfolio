# 👋 Hi, I'm Ty Kana (@Nagamiji)

### 🇰🇭 Building Production AI Systems for Khmer Language & Public Impact
> Senior Data Science Student @ ITC (GPA: 4.0) | AI Engineer | Lifelong Learner

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kana-ty-3080a42aa/)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?logo=vercel&logoColor=white)](https://portfolio-ecru-alpha-16.vercel.app/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?logo=gmail&logoColor=white)](mailto:kanaty0153@gmail.com)

---

## 🚀 Why I Build with AI

I'm passionate about **artificial intelligence** — not just as a technology, but as a tool to solve real problems for Cambodia and beyond. Every project I build teaches me something new, and I'm constantly learning, iterating, and pushing the boundaries of what's possible with machine learning.

From **Khmer handwriting recognition** to **AI-powered recruitment systems**, I love exploring how AI can make technology more accessible and impactful in low-resource settings. My drive comes from curiosity, a love for problem-solving, and the belief that AI should serve people — especially those whose languages and needs are often overlooked.

I don't just build models — I ship **production-ready AI systems** with:

✅ **MLOps rigor**: Dockerized environments, async processing, comprehensive logging  
✅ **Low-resource optimization**: 96% accuracy on Khmer digit recognition with efficient architectures (LSTM/GRU)  
✅ **Vector search expertise**: pgvector + OpenAI embeddings for semantic retrieval (10× faster queries)  
✅ **Full-stack ownership**: From data collection (Streamlit UIs) → model training → FastAPI deployment  

> *"Building AI systems for Cambodia, by Cambodia — one model at a time."*

---

## 💼 Professional Experience

### 🤖 AI Engineer @ Workingna (ATS Platform)
**July 2025 – October 2025 | Phnom Penh, Cambodia**

- Built **candidate-job matching engine** using Vertex AI embeddings and multi-vector search
- Implemented **NER with Few-Shot Learning** to extract skills and experience from resumes
- Developed **One-Click Apply Pipeline** with async processing and comprehensive logging
- Owned end-to-end ML workflows from data ingestion to model deployment

### 🔬 Project Lead & Researcher @ ITC (Khmer Penpil AI)
**March 2025 – October 2025 | Phnom Penh, Cambodia**

- Led development of **Khmer handwriting recognition system** processing 15K+ samples
- Built Streamlit web app for real-time stroke coordinate capture
- Designed **LSTM/Bi-LSTM/GRU models with attention** achieving 96% accuracy
- Created comprehensive datasets for Khmer characters, digits, and arithmetic operations

### 📊 Data Science Intern @ Scholarar (Startup)
**December 2024 – April 2025 | Phnom Penh, Cambodia**

- Developed scholarship recommendation system with **pgvector + OpenAI embeddings**
- Built automated scraping pipeline using Selenium and Playwright
- Optimized vector search with **Docker-isolated pgvector**, reducing query latency by 10×
- Worked in Agile/SCRUM environment with cross-functional teams

### 📈 Data Analyst @ Ministry of Telecommunication (MoTP)
**August 2024 – September 2024 | Phnom Penh, Cambodia**

- Built spectrum pricing model achieving **92% R² score** on 100K+ records
- Compared regression models (Linear, Ridge, Lasso, RF, SVR) with Ridge performing best
- Conducted comprehensive EDA and feature engineering for telecommunications data

---

## 📦 Featured Repositories

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

## 💡 Engineering Highlights

### 📊 Spectrum Pricing Model (MoTP Project)
```python
# Ridge regression achieved 92% R² score on 100K+ telecom records
from sklearn.linear_model import RidgeCV
model = RidgeCV(alphas=np.logspace(-3, 3, 100), cv=5)
model.fit(X_train_scaled, y_train)
print(f"R² Score: {model.score(X_test_scaled, y_test):.3f}")  # 0.921
```
✅ Clean EDA notebooks with Pandas profiling  
✅ Feature engineering documented in separate files  
✅ Model comparison across 5 algorithms (Linear/Ridge/Lasso/RF/SVR)

### ⚡ pgvector Optimization (Scholarar Internship)
```sql
-- Before: 200ms query latency
CREATE INDEX ON scholarships USING ivfflat (embedding vector_cosine_ops) 
WITH (lists = 100);

-- After: 20ms query latency (10× faster with HNSW)
CREATE INDEX ON scholarships USING hnsw (embedding vector_cosine_ops);
```
✅ Docker Compose setup for pgvector isolation  
✅ Benchmark scripts comparing IVFFlat vs HNSW indexing  
✅ OpenAPI spec for recommendation API endpoints

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
✅ Data validation to reject incomplete or malformed characters  
✅ Dataset versioning with DVC for reproducibility

### 🎯 NER with Few-Shot Learning (Workingna ATS)
```python
# Extract skills from resumes using Vertex AI + function calling
from vertexai.generative_models import FunctionDeclaration, GenerativeModel

skill_extraction = FunctionDeclaration(
    name="extract_skills",
    description="Extract technical skills and years of experience from resume text",
    parameters={...}
)

model = GenerativeModel("gemini-1.5-pro", tools=[skill_extraction])
response = model.generate_content(resume_text)
skills = response.candidates[0].function_calls[0].args
```
✅ Integrated with FastAPI for production deployment  
✅ Async processing for bulk resume parsing  
✅ Comprehensive error handling and retry mechanisms

---

## 🛠️ Tech Stack

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
![Selenium](https://img.shields.io/badge/-Selenium-43B02A?logo=selenium&logoColor=white)

### Backend & Databases
![Java](https://img.shields.io/badge/-Java-007396?logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/-Spring_Boot-6DB33F?logo=spring&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?logo=mongodb&logoColor=white)

---

## 🏆 Achievements & Leadership

🇰🇭 **ASEAN-Canada Innovative Youth Leaders Summit (ACIYLS) 2024**  
Represented Cambodia with a Reverse Vending Machine pitch converting plastic waste to energy credits

🏅 **Turing Hackathon Season 7 - Top 5 Finalist**  
Led UI/UX and market research for an AI-powered home repair platform

🔒 **Cambodia ICT Camp 2024**  
Built IoT-based security system with AI threat detection at 5-day cybersecurity bootcamp

---

## 📊 GitHub Stats

![Kana's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Nagamiji&show_icons=true&theme=radical&count_private=true&include_all_commits=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Nagamiji&layout=compact&theme=radical&langs_count=8)

---

## 🌱 Currently Learning

- Advanced NLP techniques for low-resource languages
- MLOps best practices (MLflow, model monitoring)
- Distributed training for large-scale deep learning
- Graph neural networks for recommendation systems

---

## 🤝 Let's Build Together

I'm actively seeking **Data Science / AI Engineer roles** where I can:
- Ship production ML systems with MLOps best practices
- Advance Khmer language AI (NLP/CV) for social impact
- Learn from experienced teams and contribute to meaningful projects
- Solve complex problems in public sector, edtech, or startup environments

**I'm passionate about AI, eager to learn, and ready to make an impact.**

📧 **kanaty0153@gmail.com** | 🌐 **[Portfolio](https://portfolio-ecru-alpha-16.vercel.app/)** | 💼 **[LinkedIn](https://www.linkedin.com/in/kana-ty-3080a42aa/)** | 📍 **Phnom Penh, Cambodia**

---

<div align="center">
<i>"Every line of code is a step toward making AI work for everyone — especially those who need it most."</i>
</div>
