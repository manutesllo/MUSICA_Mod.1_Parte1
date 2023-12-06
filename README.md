# Análisis de Datos de Listas de Música

Este proyecto de análisis de datos utiliza pandas y numpy para explorar un conjunto de datos que contiene estadísticas semanales de canciones en listas de música.

## Introducción

El conjunto de datos (`listas_musica.csv`) incluye las siguientes columnas:

- **date:** Fecha de la lista.
- **rank:** Posición del ranking de la canción en esa fecha.
- **song:** Nombre de la canción.
- **artist:** Artista.
- **last-week:** Posición en el ranking de la semana anterior.
- **peak-rank:** La mejor posición de la canción en el ranking.
- **weeks-on-board:** Número de semanas que la canción lleva en la lista.

## Carga de Librerías y Datos

```python
import numpy as np
import pandas as pd
import os

# Carga del dataset
file_path = "ruta/del/archivo/listas_musica.csv"
df = pd.read_csv(file_path)

# Limpieza de datos - Rellenar con 0 usando fillna()
df = df.fillna(0)

