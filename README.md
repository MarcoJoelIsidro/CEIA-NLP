# Introducción al Repositorio CEIA-NLP

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

5. En caso de que no funcione la librería tensorflow se deberá instalar manualmente con el siguiente comando dentro de poetry shell:

    ```pip install tensorflow==2.17.0 --force-reinstall```

Con estos pasos, habrá activado el entorno Poetry para ejecutar los notebooks de la materia de NLP.

## Desafíos

A continuación, se detallan los desafíos resueltos hasta el momento:

1. [Vectorización de Texto y Clasificación Naive Bayes](notebooks/01%20-%20vectorizacion%20de%20texto%20y%20clasificacion%20Naive%20Bayes/01%20-%20Resolucion.ipynb)

2. [Utilización de Gensim y análisis](notebooks/02%20-%20Custom%20embeddings%20con%20Gensim/02%20-%20Resolucion.ipynb)

3. 1. [Modelo de lenguaje con tokenizacion - char](notebooks/03%20-%20Modelo%20de%20lenguaje%20con%20tokenizacion/03%20-%20Resolucion_char.ipynb) 
   2. [Modelo de lenguaje con tokenizacion - palabras](notebooks/03%20-%20Modelo%20de%20lenguaje%20con%20tokenizacion/03%20-%20Resolucion_word.ipynb) 

4. [LSTM Bot QA](notebooks/04%20-%20LSTM%20Bot%20QA/04%20-%20Resolucion.ipynb)
