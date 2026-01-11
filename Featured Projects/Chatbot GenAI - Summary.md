# 🤖 Multi-Turn QA Chatbot with RAG and Fine-Tuned LLMs

This project centers on building a multi-turn question-answering chatbot capable of responding to user queries using real reference content. By combining fine-tuned transformer models with Retrieval-Augmented Generation (RAG), the system improves factual accuracy and reduces hallucinations compared to standalone language models.

The chatbot was designed to simulate how AI systems can assist users in navigating large text corpora, such as medical literature, technical documentation, or knowledge bases.

---

## ☁️ System Overview

The chatbot integrates three core components:

- **Fine-tuned transformer model** for answer generation  
- **Retrieval system** to select relevant context  
- **Conversation memory** to support multi-turn interactions  

Users can ask follow-up questions, and the system maintains context across multiple turns.

---

## 📊 Dataset

- Stanford Question Answering Dataset (SQuAD)  
- 100,000+ question–answer pairs  
- 500+ Wikipedia articles  
- Context-based answer extraction  

The dataset enables training models to answer questions using supporting passages rather than free-form generation.

---

## 🧠 Models

Several transformer architectures were evaluated, including:

- BERT  
- DistilBERT  
- DistilGPT-2  
- ELECTRA  
- Retro-Reader  

**ELECTRA-small** was selected due to its strong balance of accuracy, speed, and efficiency.

---

## 🔎 Retrieval-Augmented Generation (RAG)

To improve answer relevance, the system retrieves supporting text before generating responses:

- **TF-IDF** for keyword-based retrieval  
- **Sentence-BERT (SBERT)** for semantic search  

Adding SBERT improved context accuracy and reduced irrelevant passages, leading to more reliable answers.

---

## 🏆 Results

The final system demonstrated:

- Improved factual accuracy with RAG  
- Better performance with semantic retrieval  
- Stable multi-turn conversation handling  
- Reduced hallucinations compared to baseline models  

Model performance improved significantly when trained on larger portions of the dataset.

---

## 👨‍💼 My Role

- Built the chatbot interface  
- Optimized model training  
- Evaluated RAG performance  
- Conducted system testing  
- Contributed to research and documentation  

---

## 🛠️ Tech Stack

Python • PyTorch • Hugging Face Transformers  
TF-IDF • Sentence-BERT • Gradio  
Pandas • NumPy • Scikit-learn  

---

## 📫 Contact

**Ben Hopwood**  
LinkedIn: https://www.linkedin.com/in/hopwoodben  
GitHub: https://github.com/AIBenHopwood  
