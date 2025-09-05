# Portfolio

---

## Data Science (M.Sc)  
[Resume](/pdf/Lebenslauf_NhiNguyen_DS.pdf) | 📧 [Nhi.nguyenpb@gmail.com](mailto:Nhi.nguyenpb@gmail.com)  

## 📝 Projekte  
### 📚 RAG Document-Based Chatbot  

This project is a **Retrieval-Augmented Generation (RAG) chatbot** that allows users to **upload their own documents (PDF/TXT)** and and ask questions about them. The chatbot retrieves relevant document sections using embeddings and a vector database, then generates concise, context-aware answers with the help of a Large Language Model (LLM).  

***Features***
- **Upload documents** directly in the web app (PDF or TXT).  
- **Automatic document processing**: chunking, embedding, and indexing.  
- **Semantic search**: retrieve relevant chunks even if the query is paraphrased or uses synonyms.  
- **LLM-powered answers**: generates responses grounded in the uploaded content.  
- **Graceful fallback**: if the answer cannot be found in the context, the chatbot replies with *"I don’t know."*  
- **Streamlit interface**: simple and interactive UI for uploading files and chatting. 

***Example Use Cases***
- Query **research papers** or **technical reports**.  
- Extract insights from **business documents**.  
- Turn **notes** into a conversational knowledge base.  

***Tech Stack***: *Python · LangChain · FAISS · SentenceTransformers · OpenAI API · Streamlit*

![ragchatbot](/img/ragchatbot.png)
*This project demonstrates how RAG can turn static documents into interactive knowledge bases, showcasing skills in data processing, embeddings, LLM integration, and user-facing applications.*  

---

### **Data-Analyst- und Data-Science-Projekte** 
**Customer Churn Prediction**

In this project, I built a machine learning model to predict telecom customer churn and extract actionable business insights. The analysis revealed three critical risk factors driving churn: **month-to-month contracts** *(42.7%)*, **electronic check payments** *(45.3%)*, and **first-year customers** *(47.7%)*. **Fiber optic** users also showed significantly higher churn *(41.9%)*, indicating possible service or pricing issues.

Using **CatBoost** (ROC-AUC 0.85), I identified **tenure, contract type, and monthly charges** as the strongest predictors of churn. Adjusting the prediction threshold improved **campaign ROI** by enabling high-precision targeting — reducing *false positives* by *40%* while still capturing *85%* of actual churners. These insights translate into clear strategies: encourage annual contracts, shift customers to automatic payments, strengthen onboarding for new clients, and address fiber service concerns. Additionally, the churn prediction model can be leveraged to target **high-risk customers (>70% churn probability)** with *personalized offers, proactive outreach, and service guarantees*.

Implementing a strategic retention plan based on these insights could help protect **more than $1.6M in annual revenue** currently at risk.

***Skills***: *Python, Classification algorithms, Model Evaluation, Hyperparameter Tuning, Imbalanced Data, ROI Analysis*

![churn_analysis](/img/churn_analysis.png)
*Customer Churn Risk Dashboard: High-risk segments included month-to-month contracts, new customers and manual payment methods; Internet users with fiber optic also showed higher churn*

![churn_analysis](/img/churn_modeling.png)
*Churn Prediction Model Dashboard: CatBoost model performance analysis achieving 84%+ ROC-AUC with optimal business threshold (0.7)*

---

**Web Traffic Analysis and Bot Detection**

Analyzed web session data to distinguish between human users and **bot traffic** using transparent, **rule-based logic**. Developed a robust **filtering strategy** based on metadata (e.g., user agents, ASN) and behavioral signals (e.g., clickout frequency, hit volume). Built and refined **KPIs** like *Booking Conversion Rate* and *Clickout Engagement Rate* to evaluate session quality before and after filtering. Delivered a data-driven presentation with **visual and statistical comparisons**, highlighting key insights, uncovering **traffic anomalies** and providing **actionable recommendations** to improve analytics accuracy and tracking quality.

***Skills***: *Python (NumPy, Pandas , Scikit-learn, Matplotlib, Seaborn)*

***Table***: *Comparison of KPIs Before and After Bot Filtering*

| **Metric**                | **Before Filtering** | **Humans (After Filtering)** | **Bots**   |
|--------------------------|----------------------|------------------------------|------------|
| Avg. Hits/Session        | ≈64                  | <span style="color:red">≈26 ↓</span>      | ≈62    |
| Clickout Engagement Rate | 0.6%                 | <span style="color:green">33% ↑</span>    | 3.7%   |
| Booking Conversion Rate  | 0.7%                 | <span style="color:green">1% ↑</span>     | 0%     |
| Bounce Rate (1-hit)      | 23%                  | <span style="color:red">0.1% ↓</span>     | 67.9%  |

*Filtering bot traffic significantly improves the accuracy of user engagement metrics, distinguishing between real user behavior and automated activity.*

---

**Datenbasierte Analyse zur Optimierung eines Rotweinsortiments**

***Ziel:***  
Identifikation physikalisch-chemischer Eigenschaften, die mit hoher Rotweinqualität zusammenhängen, um fundierte Sortimentsentscheidungen im Handel zu unterstützen.

***Vorgehen:***  
- Explorative Datenanalyse & Korrelationsprüfung  
- Umkodierung der Qualität in zwei Klassen („gut“ vs. „nicht gut“)  
- Modellvergleich und Modellbasierte Feature-Importance: Random Forest, Gradient Boosting, SVC, Logistic Regression, KNN
- Ableitung von Schwellenwerten für die vier wichtigsten Qualitätsmerkmale

***Ergebnisse:***  
Hoch bewertete Weine zeichnen sich durch *höheren Alkoholgehalt, niedrige flüchtige Säure, moderate Sulfate und geringes Gesamtschwefeldioxid* aus. Diese Merkmale bilden eine objektive Grundlage für die Sortimentsauswahl.

***Skills***: *Python (pandas, scikit-learn, seaborn), Random Forest, Klassifikation, Feature Importance*

![Rotwein](/img/wine.png)
*Verteilung wichtiger Merkmale nach Weinbewertung (mit 1=nicht gut, 0=gut)*

---

**Produktclustering und Preismodellierung bei Tankstellen**

Im Rahmen dieses Projekts entwickelten wir datengetriebene Lösungen zur Optimierung der **Produkterfassung** und **Preismodellierung** an **Tankstellen**. Durch **Produktclustering** mittels **Konfidenzintervallen** reduzierten wir den Erfassungsaufwand um durchschnittlich **41,1%**, während wir die Genauigkeit beibehielten. Für die **Preismodellierung** nutzten wir **Gradient Boosting** und **SHAP-Werte**, um die Preisbildung zu analysieren und zu erklären, und erzielten eine signifikante Verbesserung gegenüber linearen Modellen. **Datenvorverarbeitung** und **Feature Engineering**, einschließlich der Integration von **Geodaten**, waren entscheidend für den Erfolg. Die Ergebnisse ermöglichen es der Firma, Kosten zu senken, wertvolle Einblicke in die Preisgestaltung zu gewinnen und ihre Prozesse zu optimieren. 

***Skills***: *Python, Pandas, Scikit-learn, XGBoost, SHAP, statistische Analyse, Datenvisualisierung, Projektmanagement.*

![werdenktwas](/img/werdenktwas.png)
*Ein Beispiel der Einsparung mithilfe der Produktclustering durch ähnliche Preisstrukturen*

---

### **Recommendation System** 
**Buch-Empfehlungssystem**

Dieses Projekt zielt darauf ab, ein intelligentes Empfehlungssystem für Bücher zu entwickeln, das auf den Interessen ähnlicher Nutzer:innen basiert (**Collaborative Filtering**). Die wichtigsten Schritte:

- Parsing von Buch-Metadaten
- Erstellung einer Suchmaschine zur gezielten Buchsuche  
- Identifikation von Nutzer:innen mit ähnlichen Leseinteressen**  
- Analyse der Bücher, die diesen Nutzer:innen gefallen haben  
- Generierung und Verbesserung der Empfehlungen durch Collaborative Filtering  

***Skills***: *Python (NumPy, Pandas , Scikit-learn, Matplotlib), Text Similarity Analysis, NLP (Tokenization, Tfidf)*

![BookRecommendations](/img/bookrec.png)
*Ergebnis von Buch-Empfehlungssystem mit Collaborative Filtering*

---

### **Computer Vision** 
**Qualitätssicherung von Inbusschlüsseln**

In diesem Projekt wurde ein **Computer-Vision-Programm** entwickelt, das automatisch die **Maße von Inbusschlüsseln** erfasst und im Bild ergänzt. Ziel war es, eine **kostengünstige und präzise Alternative** zur manuellen Qualitätskontrolle bereitzustellen. Das System erkennt die Werkzeuge **zuverlässig** und misst deren **Abmessungen in Millimetern**. Es ist **robust** gegenüber leichten Schatten, Bildrauschen und Variationen in der Beleuchtung. Die **Genauigkeit der Messung** wurde anhand realer Objekte überprüft und zeigte eine **geringe Abweichung** zu manuellen Messungen.

***Skills***: *Python (NumPy, Pandas, OpenCV, Matplotlib), Feature Extraction, Bildverarbeitung, Objekterkennung, Datenauswertung.*

![Ausgemessene Inbusschlüsseln](/img/cv_inbusschlüsseln.png)
*Ausgemessene Inbusschlüsseln im Bild.*

---

**Deep Learning zur automatisierten Vogelartenklassifikation**

In diesem Projekt wurde ein **Convolutional Neural Network (CNN)** zur Klassifikation von **524 Vogelarten** entwickelt. Um die Trainingsdaten zu erweitern, wurden verschiedene **Augmentierungstechniken** wie Anpassung von **Sättigung** und **Kontrast** sowie **Rotation** und **horizontales Spiegeln** angewendet.

Durch **Hyperparameter-Optimierung** wurde ein Modell mit **fünf Schichten** gefunden, das eine **Genauigkeit von 89 %** erreichte. Mithilfe von **Grad-CAM-Visualisierungen** wurde die **Erklärbarkeit** der Modellentscheidungen analysiert. Dabei zeigte sich, dass das CNN oft **Schnabel**, **Augen** oder auffällige **Farbübergänge** zur Klassifikation heranzieht. Dies führte gelegentlich zu Fehlklassifikationen, wenn nur ein einzelnes **Merkmal** betrachtet wurde. Das Projekt zeigt, dass bereits mit wenigen **Schichten** ein leistungsstarker **Klassifikator** entwickelt werden kann.

***Skills***: *Python (NumPy, Pandas, TensorFlow, OpenCV, Matplotlib), CNN, Grad-CAM, GitLab für Versionskontrolle, Statistische Evaluierung der Modellleistung,  Ergebnisvisualisierung.*

![Korrekt klassifizierter Vogel](/img/cv_vogel.png)
*Korrekt klassifizierter Vogel.*

![Falsch klassifizierter Vogel](/img/cv_vogel2.png)
*Falsch klassifizierter Vogel*

---

### **Natural Language Processing** 
**Analyse von Nachrichtenartikeln mit NLP und Web Scraping**  

Im Rahmen diese Projekts wurde einen Webcrawler entwickelt, der 1182 Artikel von *n-tv.de* heruntergeladen und in einer SQLite-Datenbank gespeichert hat. Die gesammelten Daten wurden mithilfe von NLP-Techniken analysiert, um Kategorisierungen, Wortverteilungen und Topic-Clustering zu untersuchen.  

**Hauptmethoden und Ergebnisse:**  
- **Web Scraping & Datenverarbeitung:** Extraktion von Kategorien via XPath und RegEx, Speicherung der Artikeltexte in einer Datenbank.  
- **Textanalyse:** Tokenisierung, Lemmatisierung und Berechnung der Worthäufigkeiten ergaben eine Gesamtlexikongröße von 92.475 Wörtern, die durch Vorverarbeitung auf 78.055 reduziert wurde.  
- **Ähnlichkeitsanalyse:** Berechnung von Term Frequency (TF), Inverse Document Frequency (IDF) sowie Kosinus- und Sinusähnlichkeiten zur Dokumentklassifikation. Dabei zeigte sich, dass Wirtschaftsartikel stark durch Begriffe wie „Prozent“ oder „Euro“ dominiert wurden.  
- **Topic Modeling:** Nutzung von *Latent Dirichlet Allocation (LDA)* und *BERTopic* zur automatisierten Themenextraktion. Dabei konnten Themen aus den Bereichen Wirtschaft und Gesellschaft identifiziert werden, wobei sich Cluster teilweise überlappten.  

Die Analyse zeigte, dass klassische Kategorien aus der URL nicht immer die tatsächlichen thematischen Schwerpunkte widerspiegeln. Verbesserungen könnten durch eine feinere Kategorisierung oder alternative Klassifikationsmethoden erzielt werden.

***Skills***: *Web Scraping (XPath, RegEx, BeautifulSoup, Scrapy) , Database Management (SQLite, SQL queries), NLP (Tokenization, Lemmatisation, Stopword Removal, TF-IDF), Text Similarity Analysis, Topic Modeling (LDA, BERTopic), Data Analysis (Scikit-learn, Gensim, Pandas, NumPy), Data Visualization (Matplotlib, Seaborn, Plotly), Clustering & Classification (k-Means, Neural Topic Model)*

![Clustering](/img/topic-clustering.png)
*BERTopic Modell für den ntv.de Datensatz.*

---

### **Masterarbeit: Deep Learning in EEG Classification**  
[*View Poster*](/pdf/Poster_Masterthesis_NhiNguyen.pdf)

In dieser Masterarbeit wird die Entwicklung **generalisierbarer DL-Modelle** für die Analyse von **Elektroenzephalographie (EEG)**-Daten untersucht. Ein kleines, repräsentatives **Subset** von EEG-Datensätzen wurde erstellt, das die **Diversität** einer größeren Sammlung abbildet und so die **Generalisierbarkeit** der Modelle über verschiedene EEG-Domänen hinweg fördert, ohne domänenspezifische Anpassungen zu benötigen.

Die Arbeit analysiert **11 End-to-End-DL-Modelle**, die auf **17 EEG-Datensätzen** trainiert und getestet wurden. Ein innovativer Ansatz zur Auswahl des Subsets kombiniert **Ridge-Regression** mit **Korrelationsanalysen**, um den **Median-F1-Score** der Modelle basierend auf diesem Subset vorherzusagen. Das final ausgewählte Subset minimiert **Vorhersagefehler**, gewährleistet **Diversität** und vermeidet **Redundanz**.

Die Ergebnisse zeigen, dass kein DL-Modell eine herausragende **Generalisierbarkeit** über alle Datensätze aufwies. Das ausgewählte Subset zeigte jedoch geringe **Vorhersageabweichungen** und schwache **Korrelationen**, was seine **Diversität** unterstreicht. Diese Arbeit liefert einen wertvollen **Rahmen** für die Entwicklung effizienter und **generalisierbarer DL-Modelle** in der **EEG-Klassifikation**.

***Skills***: *Deep Learning (Tensorflow/ Keras), Python, Pandas, Scikit-learn, Feature Engineering, Datenvisualisierung, Projektmanagement.*

![models](/img/ranking_models.png)
*Evaluation von Modellen: Leistung und Generalisierungsfähigkeit.*

![datasets](/img/Boxplot_datasets.png) 
*Boxplot der Modellleistung über verschiedene Datensätze.*



