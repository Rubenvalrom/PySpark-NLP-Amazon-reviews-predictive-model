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

5. **Concusión y siguientes pasos**
   - Reflexiones sobre el modelo y posibles mejoras.

## Technologías Utilizadas

Para este proyecto se ha utilizado:

- **Apache Spark 4.0.0** 
- **Hadoop 3.3.6**
- **Java 17**
- **Jupyter Notebook 7.2.2**
- **Python 3.10.18**

El resto de las dependencias están presentes en el archivo `requirements.txt`.

### Adversidades del proyecto

Cabe destacar que con esta configuración (en Windows 10) se han presentado algunas dificultades, entre ellas no poder exportar nada, esto incluye
dataframes y modelos, además de no poder trabajar con XGBoost a pesar de su adapación para Spark.

Por lo que para realizar cada sección ha sido imperativo esperar a que se ejecuten las anteriores por mucho que tarden, esto ha
sido una limitación importante, especialmente a la hora de construir un modelo más robusto.

Todas las variables de entorno estaban bien configuradas, python las reconocia y winutils.exe también funcionaba correctamente.

## Instalación de dependencias

```bash
pip install -r requirements.txt
```