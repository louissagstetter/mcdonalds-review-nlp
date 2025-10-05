# mcdonalds-review-nlp
# 🍔 McDonald's Review NLP Analysis

## 📖 Projektbeschreibung
Dieses Projekt wurde im Rahmen des IU-Moduls **"Natural Language Processing"** erstellt.  
Ziel ist es, mit NLP-Techniken die häufigsten Themen und Stimmungen aus über **33.000 McDonald's Google Reviews** aus den USA zu extrahieren.  
Das Projekt orientiert sich methodisch an der Aufgabenstellung, bei der ursprünglich Beschwerden aus einer Kommune analysiert werden sollten.

## 🎯 Ziele
- Extraktion häufig genannter Themen (Topic Modeling)
- Erkennung der allgemeinen Stimmung (Sentiment Analysis)
- Analyse von Mustern in Bewertungen (z. B. Zusammenhang zwischen Text und Sternebewertung)

## 🧰 Technologien & Bibliotheken
- **Python** 3.11  
- **Pandas**, **NumPy** – Datenaufbereitung  
- **NLTK**, **spaCy** – Textverarbeitung  
- **scikit-learn**, **gensim** – Topic Modeling & Feature Extraction  
- **TextBlob** oder **VADER** – Sentiment Analysis  
- **Matplotlib**, **pyLDAvis**, **WordCloud** – Visualisierung

## 🗂️ Projektstruktur
mcdonalds-nlp-analysis/
│
├── data/                # Datensätze
├── notebooks/           # Jupyter Notebooks
├── outputs/             # Ergebnisse & Visualisierungen
├── requirements.txt     # Bibliotheken
└── README.md            # Projektdokumentation

## 📊 Datensatz
**Quelle:** Kaggle – [McDonald's Store Reviews Dataset](https://www.kaggle.com/)  
**Umfang:** 33.000+ Google Reviews von McDonald’s Filialen in den USA  
**Spalten:**  
- `reviewer_id` – Anonymisierte ID des Rezensenten  
- `store_name`, `store_address` – Standortdaten  
- `review` – Text der Bewertung  
- `rating` – Bewertungsstern (1–5)  
- `review_time` – Zeitpunkt der Bewertung  

## 🚀 Geplante Schritte
1. Datenaufbereitung & Bereinigung  
2. Explorative Analyse  
3. Intelligente Filterung relevanter Begriffe (TF-IDF, Stopword-Tuning)  
4. Topic Modeling mit LDA + Coherence Score  
5. Sentiment-Analyse  
6. Reflexion & Interpretation

## 👤 Autor
Louis Sagstetter  
IU – Projektarbeit im Kurs *Natural Language Processing (NLP)*
