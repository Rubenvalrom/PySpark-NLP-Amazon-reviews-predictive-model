# PySpark NLP Amazon Reviews Predictive Model

Este proyecto implementa un flujo completo de Procesamiento de Lenguaje Natural (NLP) con PySpark para predecir las puntuaciones de reviews de Amazon (de 1 a 5 estrellas). Aprovecha Spark para manejar millones de registros y construir un meta-modelo predictivo.

## Secciones

1. **Análisis Exploratorio de Datos (EDA)**
   - Importación de datos con Spark.
   - Análisis de nulos y balance de clases.

2. **Procesamiento NLP**
   - Tokenización de textos.
   - Eliminación de stop-words.
   - Generación de n-gramas.
   - Vectorización con CountVectorizer y TF-IDF.

3. **Modelo Predictivo**
   - Capa 1: tres modelos base (Naive Bayes, Random Forest, Red Neuronal).
   - Capa 2: regresión logística sobre las probabilidades de los modelos base.

4. **Evaluación**
   - Error Medio Absoluto (MAE).
   - Matriz de Confusión.



