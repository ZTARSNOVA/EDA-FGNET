# Clasificación y estimación facial mediante Python para la seguridad en entornos   

El presente análisis exploratorio de datos multimedia utilizando aprendizaje estadístico y automatizado para derivar significado del modelo. En este trabajo, plantearemos algunas preguntas relacionadas con el aprendizaje en el curso y las aplicaremos a Python. En Perú, niños y jóvenes se han interesado cada vez más en crear y consumir entornos virtuales educativos y de entretenimiento. Por otro lado, la creciente exposición a contenido digital inapropiado representa un gran riesgo para el desarrollo integral.


-----------------------------------------------------

 _💡Este proyecto fue desarrollado como parte de una asignación evaluada para el curso de Análisis Exploratorio de Datos I de la Universidad San Ignacio de Loyola (USIL)._

-----------------------------------------------------

## Dataset

Este proyecto utiliza el FGNET Dataset:
- **Autor**: Aiolapo (2023)
- **Fuente**: Kaggle
- **URL**: https://www.kaggle.com/datasets/aiolapo/fgnet-dataset
- **Licencia**: MIT

<div align="center">
<img width="723" height="331" alt="dataset-cover" src="https://github.com/user-attachments/assets/6e84bec0-8038-43a8-8c68-69752dead1d7" />

</div>

## Librerías 

```python
#Librerias

import pandas as pd
import os
import matplotlib.pyplot as plt
import cv2
from PIL import Image
from pathlib import Path 
from deepface import DeepFace
from tqdm import tqdm
import seaborn as sns 

import warnings
warnings.filterwarnings('ignore')
```

## Descargar librerías 
- Permite extraer características faciales, como detectar el sexo de las imágenes del dataset FGNET

- 'tqdm' Visualizar el avance durante el análisis de las 1002 imágenes con DeepFace

```python
!pip3 install deepface tensorflow tqdm
```

