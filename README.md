# 📄 Resume Analyzer using NLP

This project is a **Resume Analyzer** built with Python and Natural Language Processing (NLP). It reads resumes in PDF format, extracts the text, processes it, and evaluates how well a resume matches a predefined list of skills and keywords. It’s useful for resume screening and basic applicant filtering.

## 🚀 Features

- 📄 PDF Resume Text Extraction  
- 🔤 Text Tokenization & Cleaning  
- 🧠 Keyword/Skill Matching  
- 📊 Resume Match Scoring  
- 🗂️ English Stopword Removal  
- 🧾 Easy-to-update Skill List  

## 🧰 Technologies Used

- Python 3.x  
- PyPDF2  
- NLTK (Natural Language Toolkit)  
- Google Colab (for Drive file access)  

## 🛠️ Setup Instructions

1. **Install dependencies**
   !pip install PyPDF

2. **Download NLTK resources**

   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   ```
## 🧪 How It Works

1. **Extract Text**
   The resume text is extracted from the PDF file using `PyPDF2`.

2. **Clean & Tokenize**
   Text is converted to lowercase, punctuation is removed, and it's tokenized using NLTK. English stopwords are also removed.

3. **Match Skills**
   Each token is checked against a predefined list of skills/keywords.

4. **Score Resume**
   Outputs:

   * The matched skills
   * A match score (number of matched keywords)
   * Percentage of relevant skills found in the resume

## 🧠 Sample Keywords List

You can modify this list as per the role or job profile. Example:

keywords = [
  "python", "data analysis", "machine learning", "deep learning",
  "artificial intelligence", "nlp", "tensorflow", "keras",
  "data visualisation", "data science", "sql", "r"
]

## ✅ Sample Output

Filtered Tokens: [....... 'nlp', '•developed', 'nlpbased', 'system', 'extract', 'analyze', 'match', 'keywords', 'resumes', 'ml'.......]
Matched_keywords: ['sql', 'nlp', 'python']
Match Score 3
Skills Found:, 3 / 271
Skills Found: 1.107011070110701 %


