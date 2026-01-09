# Transformers & LLM Lab 🚀 - Hands-on NLP with Modern Models

## 📋 Project Overview
This repository is a comprehensive lab exploring state-of-the-art transformer models for various NLP tasks. Developed as part of Bahria University's "Introduction to Data Science Lab" course, it demonstrates practical applications of:

- BART for abstractive text summarization  
- GPT-2 for creative story generation  
- Google's Gemini for conversational AI  

The project emphasizes understanding model behavior, prompt engineering, and LLM evaluation metrics.

---

## 🎯 Learning Objectives
- Implement and evaluate abstractive text summarization with BART and T5  
- Generate creative text using GPT-2 and GPT-Neo  
- Build interactive chatbots using Gemini API  
- Experiment with model parameters, prompt templates, and system prompts  
- Evaluate LLM outputs for coherence, creativity, factual accuracy, and fluency  
- Implement secure API key management  

---

## 🛠️ Tech Stack
**Core Libraries:** Transformers (Hugging Face), Google Generative AI SDK, Python-dotenv, NLTK  
**Models:**  
- **Text Summarization:** `facebook/bart-large-cnn`, `t5-base`  
- **Text Generation:** `gpt2`, `EleutherAI/gpt-neo-125M`  
- **Chatbot:** `gemini-2.5-flash`  
**Development:** Python 3.9+, Jupyter Notebook  

---

## 🔧 Installation & Setup

1. **Clone Repository**
```bash
git clone https://github.com/natashafatii/transformers-llm-lab.git
cd transformers-llm-lab
```
2. **Create Virtual Environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install Dependencies**
```bash
pip install -r requirements.txt
```

4. **Configure Environment Variables**
```bash
cp .env.template .env
# Edit .env file with your API keys
```

5. **Download NLTK Data**
```bash
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
```
## 📊 Lab Experiments & Results

###  1: **Summarization**
**Models Tested:** BART-Large-CNN, T5-Base  

**Key Findings:**  
- **BART:** Produces fluent, human-like summaries  
- **T5:** More extractive, often copies phrases  
- **Optimal Compression Ratio:** 25–30% of original text length  

---

###  2: **Creative Text Generation**
**Models Tested:** GPT-2, GPT-Neo  

**Parameter Effects:**  
- **Temperature 0.7–0.9:** Best balance between creativity and coherence  
- **Top-p 0.9:** Maintains output quality while allowing diversity  

---

###  3: **Gemini Chatbot**
**Model Used:** gemini-2.5-flash  

**Performance Metrics:**  
- **Average Response Time:** < 2 seconds  
- **Coherence:** 4.2 / 5  
- **Factual Accuracy:** 4.5 / 5  
- **User Satisfaction:** 4.3 / 5

## 🛡️ Security & Best Practices
- Use **environment variables** for API keys to keep them secure  
- Design **system prompts** for safety, specificity, and tone  
- Implement **error handling** to prevent crashes and ensure reliability  

---

## 🔮 Future Enhancements
- **Multi-modal support**: text + images  
- **Real-time streaming responses**  
- **Fine-tuning** for custom datasets  
- **Multi-language support**  
- **GUI interface** with Gradio or Streamlit  

---

## 📝 License
This project is developed for **educational purposes** as part of **Bahria University curriculum**.
