# Resume Screening & Job Recommendation App

A web application built with **Flask** and **Machine Learning** for automated resume parsing, category prediction, and job recommendation. Upload a PDF resume and instantly get:

- Predicted job category
- Extracted candidate information (name, email, phone, education, skills)
- Recommended job title based on skills and education

## Features

- **PDF Resume Upload:** Securely upload resumes in PDF format.
- **Automatic Parsing:** Extracts key information using NLP and regex.
- **Category Prediction:** Uses a trained ML model to predict the resume's job category.
- **Skill & Education Extraction:** Matches against comprehensive skill and education lists.
- **Job Recommendation:** Suggests a suitable job title based on the candidate's profile.
- **Professional UI:** Clean, responsive HTML/CSS templates.

## Quick Start

1. **Clone the repository:**
    ```sh
    git clone <repo-url>
    cd Building-Resume-Screening-App-Machine-Learning-Resume-Parsing-Resume-Job-Recommendation-Python
    ```

2. **Install dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

3. **Add your trained models:**
    - Place `rf_classifier_categorization.pkl`, `tfidf_vectorizer_categorization.pkl`, and `label_encoder.pkl` in the `models/` directory.

4. **Run the app:**
    ```sh
    python app.py
    ```

5. **Open in your browser:**
    ```sh
    $BROWSER http://localhost:5000
    ```

## Project Structure

```
├── app.py
├── models/
│   ├── rf_classifier_categorization.pkl
│   ├── tfidf_vectorizer_categorization.pkl
│   └── label_encoder.pkl
├── templates/
│   ├── index.html
│   └── result.html
├── static/
│   └── style.css
├── uploads/
├── requirements.txt
└── README.md
```

## Customization

- **Skills & Education:** Update `skills_list` and `education_keywords` in `app.py` for your domain.
- **Model:** Retrain or replace the ML model as needed.

## Requirements

- Python 3.8+
- Flask
- PyPDF2
- scikit-learn
- (See `requirements.txt` for full list)

## License

MIT License

---

*Built for automated, fair, and efficient resume screening.*