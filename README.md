# Social Media Sentiment Analysis

Proyecto de **análisis de sentimientos** en publicaciones de redes sociales utilizando técnicas de **Procesamiento de Lenguaje Natural (NLP)** y **Aprendizaje Automático**.

El objetivo es clasificar los sentimientos expresados por los usuarios en **positivos**, **negativos** y **neutros**, así como analizar el impacto de variables contextuales como la plataforma, el país y el momento de publicación.

---

## Colaboradores

- Francesca Nicole Bances Torres
- Loana Colleen Rodríguez Matos
- Cesar Rafael Sánchez Garay
  
---

## Objetivos

- Analizar sentimientos en textos provenientes de redes sociales.
- Entrenar y comparar distintos modelos de clasificación.
- Evaluar el impacto del desbalance de clases mediante técnicas de sobremuestreo.
- Identificar patrones temporales y contextuales en la expresión emocional.

---

## Dataset

- **Fuente:** Kaggle – [Social Media Sentiments Analysis Dataset](https://www.kaggle.com/datasets/kashishparmar02/social-media-sentiments-analysis-dataset)
- **Registros:** 707 publicaciones (tras limpieza)
- **Variables:** 15  
  (texto, sentimiento, plataforma, likes, retweets, país, fecha, entre otras)

---

## Preprocesamiento de Datos

- Eliminación de duplicados.
- Limpieza y normalización del texto.
- Tokenización y eliminación de *stopwords*.
- Vectorización mediante **TF-IDF**.
- Balanceo de clases con **SMOTE**.

---

## Modelos Implementados

- Naive Bayes
- Complement Naive Bayes
- Regresión Logística
- Random Forest
- Random Forest + SMOTE
- **SVM + SMOTE (mejor desempeño)**

---

## Resultados

El modelo con mejor rendimiento fue **SVM con SMOTE**, logrando:

- **Accuracy:** 78.99%
- **F1-score:** 79%
- Buen desempeño en clases minoritarias, especialmente en el sentimiento negativo.

### Comparación de Modelos

| Modelo               | Accuracy |
|---------------------|----------|
| Logistic Regression | 60.56%   |
| Random Forest       | 77.51%   |
| SVM + SMOTE         | 78.99%   |

---

## Tecnologías Utilizadas

- **Lenguaje:** Python
- **Análisis de datos:** Pandas, NumPy
- **Machine Learning:** scikit-learn
- **Balanceo de datos:** imbalanced-learn (SMOTE)
- **Visualización:** Matplotlib, Seaborn
