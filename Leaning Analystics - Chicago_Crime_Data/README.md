# 🏙️ Chicago Crime Data Analysis (PySpark)

Acest proiect analizează dataset-ul *Chicago Crime* folosind **PySpark**, tehnici Big Data și trei modele de Machine Learning.

---

## 🔧 Tehnologii folosite
- PySpark (Spark SQL & MLlib)  
- Google Colab + Google Drive  
- Matplotlib & Seaborn  
- Scikit-learn (metrici + matrice confuzie)

---

## 📂 Dataset
Dataset-ul include informații despre infracțiuni din orașul Chicago:
- `primary_type`
- `date`, `district`
- `arrest`
- `location_description`, coordonate  
Datele sunt preluate din Google Drive (`Chicago_Crime_Data.csv`).

---

## 🧼 Preprocesare
- Eliminare valori lipsă  
- Conversie `date` → timestamp  
- Extracție: `year`, `month`, `hour`, `dayofweek`  
- Conversie `arrest` din boolean → integer  
- Pregătirea datasetului pentru ML (categorice + one-hot encoding)

---

## 🔎 Analiză exploratorie (EDA)
Grafice generate:
- Top 10 tipuri de infracțiuni  
- Infracțiuni pe ani  
- Distribuția arest / ne-arest  
- Infracțiuni pe ore

---

## 🤖 Modele ML folosite
- **Logistic Regression**
- **Random Forest**
- **Gradient Boosted Trees (GBT)**

Fiecare model include:
- Matrice de confuzie  
- Classification report (precizie, recall, F1-score)  
- Accuracy   

---

## 🥇 Comparare modele
Acuratețile sunt afișate la final sub formă de listă:
- Logistic Regression: 0.8668
- Random Forest: 0.9012
- GBT: 0.9145

---

## 📌 Concluzii
Proiectul demonstrează utilizarea PySpark pentru procesarea datelor mari și antrenarea modelelor ML.  
Modelul **GBT** a obținut cea mai bună performanță și este recomandat pentru predicția probabilității unui arest.