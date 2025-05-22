# Trabajo
# Dataset de Clientes de Centro Comercial

Este repositorio contiene un dataset de clientes de un centro comercial, utilizado para realizar un análisis de segmentación (clustering). El objetivo principal del análisis fue identificar grupos de clientes con comportamientos de compra similares para poder dirigir estrategias de marketing personalizadas.

## Descripción del Dataset

El dataset `mall_customers.csv` contiene información sobre los clientes del centro comercial. Cada fila representa un cliente y las columnas incluyen las siguientes características:

* **CustomerID:** Un identificador único para cada cliente.
* **Genre:** El género del cliente (Male/Female).
* **Age:** La edad del cliente en años.
* **Annual Income (k$):** El ingreso anual del cliente en miles de dólares.
* **Spending Score (1-100):** Una puntuación asignada por el centro comercial basada en el comportamiento de gasto del cliente y la frecuencia de sus visitas (un valor más alto indica un mayor gasto).

## Análisis de Clusters

Se realizó un análisis de clustering sobre este dataset para segmentar a los clientes en grupos distintos. A continuación, se presenta un resumen de las características promedio de cada cluster identificado:

| Cluster | Genre (Promedio, 1=Male, 0=Female) | Age (Promedio) | Annual Income (k$) (Promedio) | Spending Score (1-100) (Promedio) |
| :------ | :--------------------------------: | :-------------: | :---------------------------: | :---------------------------------: |
| 0       | 0.49                               | 56.47          | 46.10                       | 39.31                               |
| 1       | 0.00                               | 39.50          | 85.15                       | 14.05                               |
| 2       | 0.00                               | 28.69          | 60.90                       | 70.24                               |
| 3       | 1.00                               | 37.90          | 82.12                       | 54.45                               |
| 4       | 1.00                               | 27.32          | 38.84                       | 56.21                               |

**Interpretación Preliminar de los Clusters:**

* **Cluster 0:** Clientes de mayor edad con ingresos anuales moderados y un puntaje de gasto relativamente bajo. Podrían ser clientes más conservadores en sus gastos.
* **Cluster 1:** Clientes exclusivamente femeninos con ingresos anuales altos pero un puntaje de gasto bajo. Podrían ser clientes ahorradores o que compran en otros lugares.
* **Cluster 2:** Clientes exclusivamente femeninos, jóvenes, con ingresos anuales moderados y un puntaje de gasto alto. Este podría ser un segmento de "compradoras frecuentes".
* **Cluster 3:** Clientes exclusivamente masculinos con ingresos anuales altos y un puntaje de gasto moderado. Podrían ser clientes que gastan de forma regular pero no impulsiva.
* **Cluster 4:** Clientes exclusivamente masculinos, jóvenes, con ingresos anuales bajos y un puntaje de gasto moderado. Podrían ser jóvenes con un potencial de crecimiento en su gasto.

## Uso del Dataset

Este dataset puede ser utilizado para:

* Experimentar con diferentes algoritmos de clustering (K-Means, DBSCAN, etc.).
* Realizar análisis exploratorio de datos (EDA) para comprender mejor las características de los clientes.
* Desarrollar estrategias de marketing segmentadas dirigidas a las necesidades específicas de cada cluster.
* Evaluar la efectividad de las campañas de marketing en diferentes segmentos de clientes.

## Contenido del Repositorio

* `mall_customers.csv`: El archivo CSV que contiene los datos de los clientes.
* `README.md`: Este archivo que proporciona una descripción del dataset y el análisis realizado.
* `Jupyternotebook.ipynb`: Archivos de código utilizados para realizar el análisis de clustering y la generación de los resultados.

## Contribuciones

Las contribuciones para mejorar la documentación o el análisis son bienvenidas. Por favor, siéntete libre de crear un "pull request" con tus sugerencias o mejoras.
