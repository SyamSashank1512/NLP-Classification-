# NLP Resume Classification & Skills Extraction

This repository contains a dynamic Natural Language Processing (NLP) application built with **Streamlit**. It enables users to upload resumes in PDF or DOCX formats and automatically analyzes the document using machine learning models and NLP toolkits (such as spaCy and NLTK). 

### Key Features
- **Resume Classification**: Predicts the job domain (e.g., PeopleSoft, SQL Developer, React JS Developer, Workday) that best matches the candidate based on their uploaded resume using a pre-trained Decision Tree model.
- **Skills Extraction**: Automatically surfaces relevant professional skills extracted from the text logic using advanced tokenization, filtering, and term matching.

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/SyamSashank1512/NLP-Classification-.git
   cd NLP-Classification-
   ```
2. Install the required python dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   *(Note: The `requirements.txt` explicitly points to the `en_core_web_sm` spaCy model. If for any reason the model fails to load, simply run `python -m spacy download en_core_web_sm` manually).*

## Usage

To launch the web interface, execute one of the python application scripts within the `Resumes` folder:

```bash
cd Resumes
streamlit run app.py
```
*(Runs the primary Resume Classification & Skills display app)*

```bash
cd Resumes
streamlit run app1.py
```
*(Runs the dedicated Skills Extraction app)*

## Folder Structure

- **`Resumes/`**: The main working directory housing Streamlit applications (`app.py`, `app1.py`), the necessary pre-trained scikit-learn machine learning vectorizer models (`.pkl`) and Decision Tree logic (`.joblib`).
- **`requirements.txt`**: Complete list of Python packages required to run the project.
- **`LICENSE`**: Open source usage rights documentation.
- **`.gitignore`**: Untracked file mappings.

---
*Created as part of an NLP & Data Science portfolio project.*
