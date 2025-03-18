# Portfolio

---

## Data Scientist (M.Sc)  
[Resume](/pdf/Lebenslauf_Nhi_Nguyen.pdf) | 📧 [Nhi.nguyenpb@gmail.com](mailto:Nhi.nguyenpb@gmail.com)  

---

## 📝 Projekte  
### **Masterarbeit: Deep Learning in EEG Classification**  
[View Poster](/pdf/Poster_Masterthesis_NhiNguyen.pdf)

In dieser Masterarbeit wird die Entwicklung generalisierbarer DL-Modelle für die Analyse von Elektroenzephalographie (EEG)-Daten untersucht, um die Herausforderungen der hohen Dimensionalität und des niedrigen Signal-Rausch-Verhältnisses zu überwinden. Ein kleines, repräsentatives Subset von EEG-Datensätzen wurde erstellt, das die Diversität einer größeren Sammlung abbildet und so die Generalisierbarkeit der Modelle über verschiedene EEG-Domänen hinweg fördert, ohne domänenspezifische Anpassungen zu benötigen.

Die Arbeit analysiert 11 End-to-End-DL-Modelle, die auf 17 EEG-Datensätzen trainiert und getestet wurden. Ein innovativer Ansatz zur Auswahl des Subsets kombiniert Ridge-Regression mit Korrelationsanalysen, um den Median-$F_1$-Score der Modelle basierend auf diesem Subset vorherzusagen. Das final ausgewählte Subset minimiert Vorhersagefehler, gewährleistet Diversität und vermeidet Redundanz.

Die Ergebnisse zeigen, dass kein DL-Modell eine herausragende Generalisierbarkeit über alle Datensätze aufwies. Das ausgewählte Subset, bestehend aus SEED, DREAMER-Valence, DREAMER-Arousal, EEGMAT und CHBMIT, zeigte jedoch geringe Vorhersageabweichungen und schwache Korrelationen, was seine Diversität unterstreicht. Diese Arbeit liefert einen wertvollen Rahmen für die Entwicklung effizienter und generalisierbarer DL-Modelle in der EEG-Klassifikation.

**Skills**: Deep Learning (Tensorflow/ Keras), Python, Pandas, Scikit-learn, Feature Engineering, Datenvisualisierung, Projektmanagement.

![models](/img/ranking_models.png)
*Evaluation von Modellen: Leistung und Generalisierungsfähigkeit.*

![datasets](/img/Boxplot_datasets.png) 
*Boxplot der Modellleistung über verschiedene Datensätze.*

### **DataScience-Projekt** 
**Produktclustering und Preismodellierung bei Tankstellen**

Im Rahmen dieses Projekts entwickelten wir datengetriebene Lösungen zur Optimierung der **Produkterfassung** und **Preismodellierung** an **Tankstellen**. Durch **Produktclustering** mittels **Konfidenzintervallen** reduzierten wir den Erfassungsaufwand um durchschnittlich **41,1%**, während wir die Genauigkeit beibehielten. Für die **Preismodellierung** nutzten wir **Gradient Boosting** und **SHAP-Werte**, um die Preisbildung zu analysieren und zu erklären, und erzielten eine signifikante Verbesserung gegenüber linearen Modellen. **Datenvorverarbeitung** und **Feature Engineering**, einschließlich der Integration von **Geodaten**, waren entscheidend für den Erfolg. Die Ergebnisse ermöglichen es der Firma, Kosten zu senken, wertvolle Einblicke in die Preisgestaltung zu gewinnen und ihre Prozesse zu optimieren. 

**Skills**: Python, Pandas, Scikit-learn, XGBoost, SHAP, statistische Analyse, Datenvisualisierung, Projektmanagement.

![werdenktwas](/img/werdenktwas.png)
*Ein Beispiel der Einsparung mithilfe der Produktclustering durch ähnliche Preisstrukturen*

### **Computer Vision** 
**Qualitätssicherung von Inbusschlüsseln**

In diesem Projekt wurde ein Computer-Vision-Programm entwickelt, das automatisch die Maße von Inbusschlüsseln erfasst und im Bild ergänzt. Ziel war es, eine kostengünstige und präzise Alternative zur manuellen Qualitätskontrolle bereitzustellen. Das System erkennt die Werkzeuge zuverlässig und misst deren Abmessungen in Millimetern. Es ist robust gegenüber leichten Schatten, Bildrauschen und Variationen in der Beleuchtung. Die Genauigkeit der Messung wurde anhand realer Objekte überprüft und zeigte eine geringe Abweichung zu manuellen Messungen.

**Skills**: Python (NumPy, Pandas, OpenCV, Matplotlib), Feature Extraction, Bildverarbeitung, Objekterkennung, Datenauswertung.

![Ausgemessene Inbusschlüsseln](/img/cv_inbusschlüsseln.png)
*Ausgemessene Inbusschlüsseln im Bild.*

**Deep Learning zur automatisierten Vogelartenklassifikation**

In diesem Projekt wurde ein Convolutional Neural Network (CNN) zur Klassifikation von 524 Vogelarten entwickelt. Um die Trainingsdaten zu erweitern, wurden verschiedene Augmentierungstechniken wie Anpassung von Sättigung und Kontrast sowie Rotation und horizontales Spiegeln angewendet.

Durch Hyperparameter-Optimierung wurde ein Modell mit fünf Schichten gefunden, das eine Genauigkeit von 89 % erreichte. Mithilfe von Grad-CAM-Visualisierungen wurde die Erklärbarkeit der Modellentscheidungen analysiert. Dabei zeigte sich, dass das CNN oft Schnabel, Augen oder auffällige Farbübergänge zur Klassifikation heranzieht. Dies führte gelegentlich zu Fehlklassifikationen, wenn nur ein einzelnes Merkmal betrachtet wurde. Das Projekt zeigt, dass bereits mit wenigen Schichten ein leistungsstarker Klassifikator entwickelt werden kann.

**Skills**: Python (NumPy, Pandas, TensorFlow, OpenCV, Matplotlib), CNN, Grad-CAM, GitLab für Versionskontrolle, Statistische Evaluierung der Modellleistung,  Ergebnisvisualisierung.

![Korrekt klassifizierter Vogel](/img/cv_vogel.png)
*Korrekt klassifizierter Vogel.*

![Falsch klassifizierter Vogel](/img/cv_vogel2.png)
*Falsch klassifizierter Vogel*

### **Natural Language Processing** 
**Analyse von Nachrichtenartikeln mit NLP und Web Scraping**  

Im Rahmen diese Projekts wurde einen Webcrawler entwickelt, der 1182 Artikel von *n-tv.de* heruntergeladen und in einer SQLite-Datenbank gespeichert hat. Die gesammelten Daten wurden mithilfe von NLP-Techniken analysiert, um Kategorisierungen, Wortverteilungen und Topic-Clustering zu untersuchen.  

**Hauptmethoden und Ergebnisse:**  
- **Web Scraping & Datenverarbeitung:** Extraktion von Kategorien via XPath und RegEx, Speicherung der Artikeltexte in einer Datenbank.  
- **Textanalyse:** Tokenisierung, Lemmatisierung und Berechnung der Worthäufigkeiten ergaben eine Gesamtlexikongröße von 92.475 Wörtern, die durch Vorverarbeitung auf 78.055 reduziert wurde.  
- **Ähnlichkeitsanalyse:** Berechnung von Term Frequency (TF), Inverse Document Frequency (IDF) sowie Kosinus- und Sinusähnlichkeiten zur Dokumentklassifikation. Dabei zeigte sich, dass Wirtschaftsartikel stark durch Begriffe wie „Prozent“ oder „Euro“ dominiert wurden.  
- **Topic Modeling:** Nutzung von *Latent Dirichlet Allocation (LDA)* und *BERTopic* zur automatisierten Themenextraktion. Dabei konnten Themen aus den Bereichen Wirtschaft und Gesellschaft identifiziert werden, wobei sich Cluster teilweise überlappten.  

Die Analyse zeigte, dass klassische Kategorien aus der URL nicht immer die tatsächlichen thematischen Schwerpunkte widerspiegeln. Verbesserungen könnten durch eine feinere Kategorisierung oder alternative Klassifikationsmethoden erzielt werden.

**Skills**: Web Scraping (XPath, RegEx, BeautifulSoup, Scrapy) , Database Management (SQLite, SQL queries), NLP (Tokenization, Lemmatisation, Stopword Removal, TF-IDF), Text Similarity Analysis, Topic Modeling (LDA, BERTopic), Data Analysis (Scikit-learn, Gensim, Pandas, NumPy), Data Visualization (Matplotlib, Seaborn, Plotly), Clustering & Classification (k-Means, Neural Topic Model)

![Clustering](/img/topic-clustering.png)
*BERTopic Modell für den ntv.de Datensatz.*


