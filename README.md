# Project Setup Guide

## Create Project Folder and Environment Setup

```bash
# Create a new project folder
mkdir <project_folder_name>

# Move into the project folder
cd <project_folder_name>

# Open the folder in VS Code
code .

# Create a new Conda environment with Python 3.10
conda create -p <env_name> python=3.10.18 -y
conda create -p env python=3.10.18 -y

# Activate the environment (use full path to the environment)
conda activate <path_of_the_env>

# Install dependencies from requirements.txt
pip install -r requirements.txt

#Crea un repo en github "DOCUMENT_PORTAL"

# Initialize Git
git init

# Verifica que tu branch local se llame "main"
git branch -M main

# Añadir remoto origin (tu repo vacío en GitHub)
git remote add origin https://github.com/pcsiemat/document_portal.git

#validation
git config --global user.name "Tu Nombre"
git config --global user.email "tunombre@gmail.com"

# Stage all files
git add .

# Commit changes
git commit -m "<write your commit message>"

# Push to remote (after adding remote origin)
git push

# Cloning the repository
git clone https://github.com/sunnysavita10/document_portal.git
```
## Minimum Requirements for the Project

### LLM Models
- **Groq** (Free)
- **OpenAI** (Paid)
- **Gemini** (15 Days Free Access)
- **Claude** (Paid)
- **Hugging Face** (Free)
- **Ollama** (Local Setup)

### Embedding Models
- **OpenAI**
- **Hugging Face**
- **Gemini**

### Vector Databases
- **In-Memory**
- **On-Disk**
- **Cloud-Based**

## API Keys

### GROQ API Key
- [Get your API Key](https://console.groq.com/keys)  
- [Groq Documentation](https://console.groq.com/docs/overview)

### Gemini API Key
- [Get your API Key](https://aistudio.google.com/apikey)  
- [Gemini Documentation](https://ai.google.dev/gemini-api/docs/models)


# Dev
  folder
   archive
   data
   faiss_index
   logs
  file
   .env

# Go to execute 
       "uvicorn api.main:app --reload"
       "uvicorn api.main:app --port 8080 --reload"
       "uvicorn api.main:app --host 0.0.0.0 --port 8080 --reload"