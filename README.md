# French Resumes NER Model
## Overview
This project features a **SpaCy Named Entity Recognition (NER) model** designed to extract key information from **French resumes (CVs) and job postings**. It automates candidate screening by identifying crucial details such as **job titles, skills, experience, education, and contact information**.

## Features 
- Detects key **entities** in resumes and job offers.
- Supports **French language**.
- Helps in **recruitment automation**.
- Can be integrated into **AI-driven hiring tools**.

## Entities Extracted 
- **DIPLOME** (Degree) 🎓
- **POSTE** (Job Title) 💼
- **CONTACT** (Contact Information) 📞
- **CERTIFICATION** (Certifications)
- **EXPERIENCE** (Experience) 📊
- **COMPETENCES** (Skills) 🛠️

## Dataset 
The model was trained on **French resumes and job postings** collected from various sources, ensuring a diverse and high-quality dataset. The dataset includes **CVs** and **job postings** from multiple industries.

## Installation 
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/french-resumes-ner.git
   cd french-resumes-ner
   ```
2. Download the trained SpaCy model:
   ```bash
   spacy download fr_core_news_md
   ```

## Usage 
```python
import spacy
nlp = spacy.load("path/to/your/model")
text = "Jean Dupont est un Data Scientist basé à Paris. Il maîtrise Python et possède une certification TensorFlow."
doc = nlp(text)
for ent in doc.ents:
    print(ent.text, ent.label_)
```

## Training 
To train the model from scratch:
```bash
python train_ner.py
```

## Future Improvements 
- Expand dataset with more **domain-specific resumes**.
- Improve accuracy with **fine-tuning on niche job sectors**.
- Integrate **real-time video analysis for interview insights**.

## License 
This project is licensed under the **MIT License**.

## Contributions 
Feel free to **fork, improve, and contribute**! 🚀

