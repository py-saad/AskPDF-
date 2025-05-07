# AskPDF - PDF Q&A System

![Project Logo](media/logo.png) *(optional)*

## 📌 Overview
A Django-based web application that allows users to:
- Upload PDF documents
- Automatically process and index content
- Ask questions about uploaded documents
- Get AI-generated answers based on document content

## 🌟 Key Features
- PDF text extraction and processing
- Lightweight AI model for text generation
- Context-aware question answering
- User authentication
- Document management

## 🛠️ Tech Stack
- **Backend**: Django 4.2+
- **AI Models**: 
  - Sentence Transformers (for embeddings)
  - DistilGPT-2/TinyLLaMA (for text generation)
- **Database**: SQLite (default) / PostgreSQL
- **Frontend**: HTML5, Bootstrap 5, JavaScript

## 🚀 Installation (Windows)

### Prerequisites
- Python 3.9+
- Git (optional)
- Virtual Environment

### Setup Steps
```cmd
:: 1. Clone repository (if applicable)
git clone https://github.com/yourusername/askpdf.git
cd askpdf

:: 2. Create and activate virtual environment
python -m venv venv
venv\Scripts\activate

:: 3. Install dependencies
pip install -r requirements.txt

:: 4. Configure environment variables
copy config\sample_env.py config\local_settings.py

:: 5. Apply migrations
python manage.py migrate

:: 6. Create superuser
python manage.py createsuperuser

:: 7. Run development server
python manage.py runserver
