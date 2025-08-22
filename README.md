# Intelligent Document Assistant  

A lightweight but practical AI tool that allows users to interact with documents and web content. Built using **Python, LangChain, and Streamlit**, and powered by a **locally running Mistral 7B LLM** for privacy and efficiency.  

## Overview  

This app processes user-provided **documents** (PDF, DOCX, TXT) or **URLs** and enables intelligent Q&A over the content. Users can upload files or paste links, and the system extracts and analyzes the information so they can ask natural language questions and get context-aware answers.  

I built this in a couple of days in my free time to practice building LLM-powered tools and improve my Python and LangChain skills.  

## Features  

- **Document & URL support** – upload PDF, DOCX, TXT files, or paste a web link  
- **Interactive Q&A** – ask natural language questions about your content  
- **Local model** – runs on **Mistral 7B**, an open-source language model with 7 billion parameters designed for text understanding and question answering  
- **Streamlit-based UI** – clean, simple, and interactive frontend  
- **No external API dependency** – keeps data private and reduces cost  

## Tech Stack  

- **Language:** Python  
- **Frameworks:** Streamlit, LangChain  
- **Model:** [Mistral 7B LLM](https://mistral.ai/) (open-source, locally hosted from Ollama)  
- **Libraries:** llama-cpp-python, PyPDF2, docx2txt, requests  

## Installation & Setup  

1. **Clone this repository**  
   ```bash
   git clone https://github.com/zaraazaman/intelligent-document-assistant.git
   cd intelligent-document-assistant
2. **Create and activate a virtual environment** (recommended)
   ```python -m venv venv
    # Windows
    venv\Scripts\activate
    # Mac/Linux
    source venv/bin/activate
3. **Install dependencies**
    pip install -r requirements.txt
4. **Run the Streamlit app**
    streamlit run app.py
5. **Open in browser**
Visit http://localhost:8501

# How It Works
1. Upload documents or paste URLs

2. The app extracts and preprocesses text

3. LangChain pipelines route the content to the local Mistral model

4. Users can interact through a Streamlit interface

# Screenshots
<img width="1912" height="957" alt="interface3" src="https://github.com/user-attachments/assets/29de6cba-2171-486e-a628-4e94fdbe3a63" />
<img width="1901" height="944" alt="interface2" src="https://github.com/user-attachments/assets/dbb5745a-e751-4778-8e2b-4043051e2a82" />
<img width="1909" height="958" alt="interface1" src="https://github.com/user-attachments/assets/d1c58506-00eb-411f-b50f-03b7fe62d207" />

# Future Improvements
1. Add search highlighting: Highlight query-relevant text in the uploaded documents to improve user experience.
2. Enhance multi-document features: While multiple document upload is supported, future iterations could improve speed and accuracy with larger datasets.
3. Expand history features: The Q&A history is saved, but future versions could include user authentication and cloud storage for persistent access across devices.
