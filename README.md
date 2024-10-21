# Introducción al Repositorio CEIA-NLP

![BannerUBA](logoFIUBA.jpg)

![Poetry](https://img.shields.io/badge/poetry-1C9C8F?style=for-the-badge&logo=poetry&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)

Integrante: Isidro, Marco Joel

Este repositorio contiene los notebooks y desafíos correspondientes a la materia de Procesamiento del Lenguaje Natural (NLP) de la especialización en Inteligencia Artificial (CEIA) de la UBA.

## Estructura de Directorios

El repositorio está organizado de la siguiente manera:

```
├── notebooks/
│   ├── 01 - vectorizacion de texto y clasificacion Naive Bayes/
│   │   ├── 01 - Enunciado.ipynb
│   │   └── 01 - Resolucion.ipynb
│   ├── desafio2
│   ├── ...
│   └── desafioN
└── README.md
```

En el directorio `notebooks/` se encuentran los notebooks correspondientes a cada desafío de la materia. Cada desafío tiene su propio directorio, dentro del cual se encuentran los archivos `0x - Enunciado.ipynb` y `0x - Resolucion.ipynb`. El primero contiene el enunciado del desafío brindado por la cátedra, mientras que el segundo contiene la resolución del desafío.

## Activar el entorno Poetry

Para activar el entorno Poetry y asegurarse de tener todas las dependencias necesarias instaladas, siga los siguientes pasos:

1. Asegúrese de tener Poetry instalado en su sistema. Si no lo tiene, puede instalarlo siguiendo las instrucciones en [https://python-poetry.org/docs/](https://python-poetry.org/docs/).

2. Navegue hasta la raíz del repositorio en su terminal.

3. Ejecute el siguiente comando para instalar las dependencias necesarias:
    
    ```poetry install```

4. Active el entorno Poetry ejecutando el siguiente comando:

    ```poetry shell```

5. En caso de que no funcione la librería tensorflow con GPU se deberá instalar manualmente con el siguiente comando dentro de poetry shell:

    ```pip install tensorflow==2.15.0 --force-reinstall```

Con estos pasos, habrá activado el entorno Poetry para ejecutar los notebooks de la materia de NLP.

>info: en caso de trabajar en windows se recomienda la utilización de WSL para evitar problemas de instalación con tensorflow

## Desafíos

A continuación, se detallan los desafíos resueltos hasta el momento:

1. [Vectorización de Texto y Clasificación Naive Bayes](notebooks/01%20-%20vectorizacion%20de%20texto%20y%20clasificacion%20Naive%20Bayes/01%20-%20Resolucion.ipynb)

En este desafío se utiliza el conjunto de datos 20 newsgroups, que contiene una colección de noticias clasificadas en diferentes categorías, para explorar y aplicar técnicas de vectorización de texto. Posteriormente, se entrenan modelos de clasificación, como Naïve Bayes, para evaluar cómo estos métodos de vectorización influyen en la capacidad del modelo para clasificar correctamente los documentos en sus respectivas categorías.

2. [Utilización de Gensim y análisis](notebooks/02%20-%20Custom%20embeddings%20con%20Gensim/02%20-%20Resolucion.ipynb)

Se lleva a cabo un desafío que implica la creación de vectores de palabras utilizando la librería Gensim y el modelo Word2Vec, aplicando estas técnicas sobre el texto de la novela "Los Miserables" de Victor Hugo. El proceso incluye un preprocesamiento del texto, como la limpieza y tokenización, seguido por la generación de embeddings de palabras a partir del corpus literario. Además, se proponen pruebas de similitud entre términos y tests de analogías utilizando estos embeddings. Finalmente, se plantea la visualización de los resultados y se extraen conclusiones sobre las relaciones semánticas encontradas.

3. 1. [Modelo de lenguaje con tokenizacion - char](notebooks/03%20-%20Modelo%20de%20lenguaje%20con%20tokenizacion/03%20-%20Resolucion_char.ipynb) 
   2. [Modelo de lenguaje con tokenizacion - palabras](notebooks/03%20-%20Modelo%20de%20lenguaje%20con%20tokenizacion/03%20-%20Resolucion_word.ipynb) 

En este desafío se trabajó con el texto de una obra literaria de Julio Verne. El objetivo principal fue construir representaciones vectoriales de palabras y desarrollar un modelo de lenguaje basado en caracteres, lo cual permitió analizar tanto las relaciones semánticas a nivel de palabra como la capacidad del modelo para generar texto de manera coherente.

* Generación de embeddings de palabras: Se aplicaron técnicas de Word Embeddings para representar las palabras del libro en vectores densos, capturando así las relaciones semánticas entre ellas según su contexto en el texto literario. Usando modelos como Word2Vec, se logró que las palabras frecuentemente asociadas en la narrativa compartieran una cercanía en el espacio vectorial. Esto ayudó a identificar patrones temáticos y de estilo en la obra.

* Modelo de lenguaje basado en caracteres: Además de los embeddings de palabras, se construyó un modelo de lenguaje que trabaja a nivel de caracteres. Este enfoque permitió entrenar una red neuronal recurrente (como LSTM o GRU) que es capaz de predecir secuencias de texto a partir de contextos previos, aprendiendo el flujo y estilo de escritura característico de Julio Verne. Para la generación de nuevas secuencias, se probaron diversas estrategias, como greedy search y beam search (determinístico y estocástico), ajustando la temperatura para observar cómo afecta la creatividad y diversidad de los textos generados.

Este enfoque combinado permitió capturar tanto la semántica de alto nivel entre las palabras como la estructura detallada de las secuencias de caracteres, logrando que el modelo pudiera tanto entender el contexto como generar texto nuevo de manera coherente con el estilo del autor.

4. [LSTM Bot QA](notebooks/04%20-%20LSTM%20Bot%20QA/04%20-%20Resolucion.ipynb)

Este desafío se centra en la creación de un bot de preguntas y respuestas (QA) utilizando los datos del Second Conversational Intelligence Challenge (ConvAI2), que contiene diálogos en inglés. El bot es capaz de interpretar y responder preguntas formuladas por el usuario basándose en conversaciones previas. El enfoque principal consiste en entrenar el modelo para que comprenda el contexto de las conversaciones y genere respuestas coherentes y relevantes, utilizando técnicas de procesamiento de lenguaje natural y modelos de lenguaje avanzados.

5. [Bert Sentiment Analysis](notebooks/05%20-%20Bert%20Sentiment%20Analysis/05%20-%20Resolucion.ipynb)

En este desafío, se entrena un modelo basado en BERT (Bidirectional Encoder Representations from Transformers) para realizar análisis de sentimiento sobre un dataset de reseñas de aplicaciones. El modelo de BERT se utiliza como encoder, lo que permite capturar de manera efectiva el contexto bidireccional de las palabras en las reseñas, mejorando la precisión en la clasificación del sentimiento (positivo, negativo, neutral) expresado por los usuarios. Este enfoque permite obtener una comprensión profunda del sentimiento detrás de cada reseña, utilizando una arquitectura de última generación en NLP.
Además se utilizaron las 5 categorias originales del dataset para el entrenamiento de un nuevo modelo.