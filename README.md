# Analisis-de-Redes-Sociales

Este proyecto implementa un análisis básico de una red social a partir de un conjunto de datos de interacciones. Utiliza las bibliotecas `pandas` para la manipulación de datos, `networkx` para la creación, manipulación y estudio de la estructura y dinámica de redes complejas, y `matplotlib` para la visualización de la red.

## Descripción del Proyecto

El script en el Jupyter Notebook `Analisis de Redes Sociales.ipynb` lleva a cabo los siguientes pasos:
1.  Carga de un conjunto de datos de interacciones desde un archivo CSV (`networks_2019.csv`).
2.  Construcción de un grafo no dirigido donde los nodos representan usuarios/entidades y las aristas ponderadas representan la fuerza de la interacción entre ellos.
3.  Cálculo y visualización de estadísticas básicas del grafo, como el número de nodos y aristas.
4.  Cálculo de la centralidad de grado para identificar los nodos más influyentes o conectados en la red.
5.  Extracción y visualización de un subgrafo compuesto por los nodos más centrales.
6.  Análisis de los componentes conectados de la red, identificando el tamaño del componente más grande.
7.  Cálculo de la densidad de la red para entender qué tan conectada está.
8.  Cálculo del diámetro del componente principal, que indica la "distancia" máxima entre dos nodos en dicho componente.

## Características Principales / Análisis Realizado

* **Carga de Datos:** Importación de datos de la red desde un archivo CSV.
* **Construcción del Grafo:** Creación de un grafo no dirigido y ponderado usando NetworkX.
* **Métricas Básicas:**
    * Número de nodos (usuarios/entidades).
    * Número de aristas (interacciones).
* **Análisis de Centralidad:**
    * Cálculo de la centralidad de grado.
    * Identificación de los 5 usuarios más centrales.
* **Visualización:**
    * Visualización de un subgrafo de los usuarios más centrales.
* **Análisis Estructural:**
    * Detección de componentes conectados.
    * Cálculo del tamaño del componente más grande.
    * Cálculo de la densidad de la red.
    * Cálculo del diámetro del componente principal.
 
## Conjunto de Datos

El análisis se basa en el archivo `networks_2019.csv`. Se espera que este archivo contenga al menos las siguientes columnas para representar las aristas de la red:
* `node_1`: El nodo origen de la interacción.
* `node_2`: El nodo destino de la interacción.
* `weighted`: El peso o la fuerza de la interacción entre `node_1` y `node_2`.

## Requisitos

Para ejecutar este proyecto, necesitarás tener instaladas las siguientes bibliotecas de Python:
* pandas
* networkx
* matplotlib
