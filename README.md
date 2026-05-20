Sentiment Analysis on Kindle Reviews
Este proyecto trata sobre un análisis de sentimientos usando reseñas de Kindle. La idea principal fue aplicar técnicas de NLP y Machine Learning para que el sistema pudiera identificar si una reseña tiene un sentimiento positivo o negativo.
Integrantes
Daniela Abarca
Elizabeth Vizcarra
Daniela Rodríguez
Tecnologías utilizadas
Python
Pandas
NLTK
Scikit-learn
Matplotlib
Modelos utilizados
Logistic Regression
Random Forest
Estructura del proyecto
data/
notebooks/
src/
results/
Objetivo
El objetivo de este proyecto fue construir un sistema de Sentiment Analysis utilizando reseñas reales de Kindle. Para lograrlo, se trabajó con técnicas de procesamiento de lenguaje natural, desde la limpieza del texto hasta el entrenamiento de modelos de clasificación.
Durante el proyecto se aplicaron pasos como tokenización, eliminación de stopwords, stemming, lemmatization, Bag of Words, TF-IDF y evaluación de modelos. Al final, el sistema busca clasificar las reseñas como:

Positivas
Negativas
Dataset utilizado
Se utilizó el dataset Amazon Reviews: Kindle Story Category, disponible en Kaggle.
Este dataset contiene reseñas de usuarios sobre libros Kindle, y nos sirvió como base para entrenar y probar los modelos.

Proceso realizado
El proyecto se desarrolló siguiendo un flujo completo de NLP:
Primero se cargó y revisó el dataset.
Después se limpió el texto, quitando signos de puntuación, caracteres especiales y convirtiendo todo a minúsculas.
Se aplicó tokenización para separar las palabras.
Se eliminaron stopwords para quitar palabras que no aportaban mucho al análisis.
Se usaron técnicas como stemming y lemmatization para normalizar las palabras.
Luego se transformó el texto a valores numéricos usando Bag of Words y TF-IDF.
Se dividieron los datos en entrenamiento y prueba.
Se entrenaron los modelos.
Finalmente, se evaluaron los resultados y se comparó el desempeño.
Representaciones utilizadas
Para que los modelos pudieran trabajar con texto, fue necesario convertir las reseñas en datos numéricos. Para esto se usaron dos métodos:
Bag of Words:
Cuenta cuántas veces aparece cada palabra dentro del texto.

TF-IDF:
Toma en cuenta la importancia de una palabra dentro de una reseña y dentro de todo el dataset, por lo que ayuda a darle más peso a palabras relevantes.

Evaluación de modelos
Los modelos se evaluaron usando diferentes métricas:
Accuracy
Precision
Recall
F1-score
Matriz de confusión
Estas métricas nos ayudaron a ver qué tan bien estaba clasificando cada modelo y cuál tuvo mejor rendimiento.
Análisis comparativo
Durante el proyecto se compararon diferentes técnicas y modelos para identificar cuál funcionaba mejor.
Se comparó Bag of Words contra TF-IDF, ya que ambas técnicas convierten texto en datos numéricos, pero lo hacen de manera diferente. Bag of Words se basa en contar palabras, mientras que TF-IDF toma en cuenta la importancia de cada palabra dentro del texto.

También se comparó el uso de stemming y lemmatization, ya que ambos ayudan a reducir palabras a una forma más simple, aunque lemmatization suele conservar mejor el significado de las palabras.

Finalmente, se compararon los modelos entrenados para revisar cuál obtuvo mejores resultados con las métricas de evaluación.

Uso general de Inteligencia Artificial
Durante el desarrollo del proyecto se utilizó Inteligencia Artificial como una herramienta de apoyo para resolver dudas, organizar ideas y mejorar algunas partes de la documentación. Su uso no fue para realizar todo el proyecto, sino para complementar el trabajo del equipo.
En general, la IA se utilizó para comprender mejor algunos conceptos de NLP, revisar la estructura del pipeline, apoyar en ejemplos de limpieza de texto, explicar técnicas como Bag of Words y TF-IDF, y mejorar la redacción de la documentación.

Aproximadamente el 15% del código fue apoyado por IA, por lo que no se superó el límite permitido del 30%. Todo el código utilizado fue revisado, probado y entendido por el equipo antes de integrarlo al proyecto.

Pruebas realizadas
Se probó cada parte del proyecto para verificar que funcionara correctamente:
Carga del dataset.
Limpieza del texto.
Tokenización.
Eliminación de stopwords.
Transformación con BoW y TF-IDF.
Entrenamiento de modelos.
Evaluación con métricas.
También se revisaron los resultados para comprobar si los modelos estaban clasificando correctamente las reseñas positivas y negativas.
Errores encontrados
Durante el desarrollo aparecieron algunos problemas, por ejemplo:
Reseñas con caracteres especiales.
Palabras que no aportaban información útil.
Diferencias entre los resultados obtenidos con BoW y TF-IDF.
Algunas reseñas eran difíciles de clasificar porque podían ser ambiguas.
Cómo se corrigieron
Para corregir estos problemas, se mejoró la limpieza del texto, se eliminaron stopwords y se compararon diferentes formas de representar las reseñas. También se probaron distintos modelos para ver cuál daba mejores resultados.
Conclusión
Este proyecto nos ayudó a entender cómo se puede aplicar NLP para analizar sentimientos en textos reales. Se logró crear un proceso completo, desde la limpieza de las reseñas hasta la evaluación de modelos de Machine Learning.
También se compararon técnicas como Bag of Words y TF-IDF, además de diferentes modelos de clasificación. El uso de IA fue limitado a aproximadamente 15% del código, usándose solo como apoyo para organizar, entender y documentar mejor el proyecto.

