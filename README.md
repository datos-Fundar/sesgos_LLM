![](https://fund.ar/wp-content/uploads/2024/03/FU_Portada_Sesgos.jpg)

Este repositorio forma parte del documento de trabajo [Sesgos algorítmicos y representación social en los modelos de lenguaje generativo (LLM)](https://fund.ar/publicacion/sesgos-algoritmicos-y-representacion-social-en-los-modelos-de-lenguaje-generativo/) publicado por el [equipo de Datos de Fundar](https://fund.ar/area/datos/). Este artículo se fundamenta en los hallazgos presentes en este [artículo](https://arxiv.org/pdf/2303.17548.pdf) publicado por la Universidad de Stanford que utilizó el conjunto de datos [OpinionQA](https://paperswithcode.com/dataset/opinionqa) y la metodología para evaluar Modelos de Lenguaje (LMs) mediante encuestas de opinión pública. 

Aplicamos un enfoque similar para explorar cómo los LMs reflejan y se alinean con las opiniones de diversos grupos demográficos en el contexto argentino. A partir de preguntas adaptadas de encuestas de [Latinobarómetro](https://www.latinobarometro.org/lat.jsp), abordamos temas relevantes para el panorama sociopolítico argentino y analizamos el alineamiento de las respuestas de los LMs con diferentes segmentos de la población. Nuestro objetivo fue revelar posibles sesgos y discrepancias, proporcionando una comprensión matizada de cómo estos modelos interpretan opiniones en el contexto específico de Argentina.

El propósito de este repositorio es permitir a cualquier persona replicar el trabajo realizado. 

## Organización del proyecto:

En [`datasets`](./datasets/) se encuentran los datos de Latinobarómetro utilizados para promptear a los modelos y evaluar las respuestas.

En [`outputs`](./outputs/) se encuentran los resultados de los distintos scripts y notebooks. (A destacar, los gráficos generados y las respuestas consolidadas de cada modelo).

El análisis está repartido entre las Jupyter Notebooks y los [scripts](./scripts/).
En particular:
  - `bard.ipynb`, `chatgpt.ipynb`, y `cohere.ipynb` contienen las notebooks donde se promptean a los correspondientes modelos con las preguntas seleccionadas.
  - Las notebooks `distances_` contienen el cálculo de las distancias de opinión correspondientes a cada modelo.
  - En `scripts/multivariado.R` se realizan los modelos de regresión lineal ajustados a través de OLS para el análisis multivariado.

    
