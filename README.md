# mcdonalds-review-nlp
# 🍔 McDonald's Review NLP Analysis

🧠 NLP Textanalyse – McDonald’s Reviews (IU Projekt: Data Analysis)

Dieses Projekt wurde im Rahmen des IU-Fernstudiums Cyber Security im Modul Projekt: Data Analysis umgesetzt.
Ziel war es, mithilfe von Natural Language Processing (NLP) unstrukturierte Textdaten automatisiert zu analysieren und daraus Themen und Stimmungen zu erkennen.

## 📖 Projektbeschreibung
Dieses Projekt wurde im Rahmen des IU-Moduls **"Natural Language Processing"** erstellt.  
Ziel ist es, mit NLP-Techniken die häufigsten Themen und Stimmungen aus über **33.000 McDonald's Google Reviews** aus den USA zu extrahieren.  
Das Projekt orientiert sich methodisch an der Aufgabenstellung, bei der ursprünglich Beschwerden aus einer Kommune analysiert werden sollten.

Im Szenario sollten ursprünglich Beschwerden einer Kommune analysiert werden.
Da diese Daten nicht öffentlich zugänglich sind, wurde stattdessen ein vergleichbarer offener Datensatz von über 33.000 Google Reviews von McDonald’s-Filialen in den USA verwendet (Quelle: Kaggle).

Projektbeschreibung
Die Daten enthalten zahlreiche Kundenbeschwerden, Kritikpunkte und Feedback, die methodisch ähnliche Strukturen aufweisen wie die im Szenario beschriebenen kommunalen Beschwerdedaten.


## 🎯 Ziele
- Extraktion häufig genannter Themen (Topic Modeling)
- Erkennung der allgemeinen Stimmung (Sentiment Analysis)
- Analyse von Mustern in Bewertungen (z. B. Zusammenhang zwischen Text und Sternebewertung)

Zielsetzung

Ziel des Projekts war es:
	•	unstrukturierte Textdaten zu bereinigen und vorzubereiten,
	•	Sentiment-Analysen durchzuführen,
	•	mithilfe von LDA-Topic-Modeling wiederkehrende Themen zu erkennen,
	•	die Ergebnisse visuell und interpretativ aufzubereiten.


## 🧰 Technologien & Bibliotheken
- **Python** 3.11  
- **Pandas**, **NumPy** – Datenaufbereitung  
- **NLTK**, **spaCy** – Textverarbeitung  
- **scikit-learn**, **gensim** – Topic Modeling & Feature Extraction  
- **TextBlob** oder **VADER** – Sentiment Analysis  
- **Matplotlib**, **pyLDAvis**, **WordCloud** – Visualisierung

Methodik und Tools

Programmiersprache:
	•	Python 3.9

Verwendete Bibliotheken:
	•	pandas, numpy – Datenanalyse
	•	nltk, spacy – NLP (Tokenisierung, Lemmatisierung, Stopwords)
	•	scikit-learn, gensim – Vektorisierung, Topic Modeling
	•	matplotlib, pyLDAvis – Visualisierung

Analyse-Schritte:
	1.	Datenbereinigung: Entfernen von Sonderzeichen, URLs, Zahlen, Stopwords
	2.	Tokenisierung & Lemmatisierung: Vereinheitlichung der Wortformen
	3.	Sentiment-Analyse: Bewertung der Textstimmung (negativ → positiv)
	4.	Topic Modeling (LDA): Extraktion der häufigsten Themen
	5.	Evaluation: Optimierung mit Coherence Score


📊 Ergebnisse

Top 5 identifizierte Themen:
	1.	Bestell- und Wartezeiten („hour“, „order“, „time“)
	2.	Service und Sauberkeit („friendly“, „clean“, „staff“, „good“)
	3.	Negative Erfahrungen („terrible“, „dirty“, „fry“)
	4.	Positive Erlebnisse („happy“, „excellent“, „meal“)
	5.	Drive-Thru & Kundenservice („rude“, „manager“, „line“, „drive“)

Sentiment-Ergebnisse (Durchschnitt je Sternebewertung):
Bewertung
Sentiment-Durchschnitt
⭐ 1
−0.20
⭐ 2
−0.08
⭐ 3
+0.10
⭐ 4
+0.38
⭐ 5
+0.52


## 🗂️ Projektstruktur
mcdonalds-nlp-analysis/
│
├── data/                # Datensätze
│   ├── mcdonalds_reviews.csv
│   ├── verarbeitete_daten.csv
├── notebooks/           # Jupyter Notebooks
│   ├── phase1_konzept.ipynb
├── outputs/             # Ergebnisse & Visualisierungen
│   ├── sentiment_distribution.png
│   ├── top20_words.png
│   ├── lda_topics.png
│   ├── topic_words.csv
│   └── sentiment_summary.csv
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

💬 Reflexion

Dieses Projekt zeigt, wie NLP-Methoden helfen können, große Mengen unstrukturierter Texte effizient zu analysieren.
Die Kombination aus Sentiment-Analyse und Topic Modeling liefert wertvolle Einblicke in Kundenmeinungen und ermöglicht datenbasierte Entscheidungen – sowohl im privaten Sektor als auch in kommunalen Kontexten.

📚 Quellen
	•	Datensatz: McDonald’s Store Reviews (Kaggle)
	•	Bibliotheken: NLTK, gensim, scikit-learn
	•	Lehrmaterial: IU Modul „Projekt: Data Analysis“
  
## 👤 Autor
Louis Sagstetter  
IU – Projektarbeit im Kurs *Natural Language Processing (NLP)*
