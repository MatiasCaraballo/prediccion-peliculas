# 🎬 Predicción de Premios Oscar

Este proyecto utiliza machine learning para predecir si una película ganará premios Oscar basándose en sus características como géneros, calificaciones y reseñas.

El dataset utilizado para el proyecto es : 

"IMDb Top 100 Movies Dataset (2025 Edition)" de shayanzk : 

https://www.kaggle.com/datasets/shayanzk/imdb-top-100-movies-dataset-2025-edition

License: Creative Commons Attribution 4.0 International (CC BY 4.0)


## 🚀 Instalación y Configuración

### 1. Clonar el Repositorio

```bash
git clone https://github.com/MatiasCaraballo/prediccion-peliculas.git
cd prediccion-peliculas
```

### 2. Crear Entorno Virtual

#### En Windows:
```bash
python -m venv venv
venv\Scripts\activate
```

#### En macOS/Linux:
```bash
python3 -m venv venv
source venv/bin/activate
```


### 3. Instalar Dependencias

Una vez activado el entorno virtual, instala todas las dependencias necesarias:

```bash
pip install -r requirements.txt
```



### Funcionalidades del Proyecto

El notebook incluye tres modelos de predicción:

1. **Predicción Completa**: Usa todos los features (géneros + reseñas)
2. **Predicción por Géneros**: Solo considera los géneros de la película
3. **Predicción por Reseñas**: Solo considera calificaciones y métricas


## 📈 Dataset

Este proyecto utiliza el dataset **"IMDb Top 100 Movies Dataset (2025 Edition)"** de Kaggle:

- **Autor**: shayanzk
- **URL**: https://www.kaggle.com/datasets/shayanzk/imdb-top-100-movies-dataset-2025-edition
- **Licencia**: Creative Commons Attribution 4.0 International (CC BY 4.0)

### Cambios Realizados en el Dataset

- **Limpieza de datos**: Eliminación de columnas irrelevantes
- **Feature Engineering**: Codificación one-hot de géneros usando `MultiLabelBinarizer`
- **Preprocesamiento**: Conversión a matrices numpy para machine learning

### Variables del Dataset

- **Year**: Año de lanzamiento
- **IMDb Rating**: Calificación en IMDb
- **Rotten Tomatoes %**: Porcentaje de aprobación en Rotten Tomatoes
- **Runtime**: Duración en minutos
- **Metacritic**: Puntuación en Metacritic
- **Oscars Won**: Número de premios Oscar ganados (variable target)
- **Genres**: Géneros de la película (codificados como variables dummy)


### Estructura del Proyecto

```
prediccion-peliculas/
├── main.ipynb              # Notebook principal con análisis y modelos
├── requirements.txt         # Dependencias del proyecto
├── README.md               # Esta documentación
├── LICENCE_DATA.md         # Información de licencias del dataset
├── venv/                   # Entorno virtual (no versionado)
└── .gitignore             # Archivos ignorados por Git
```

## 📝 Licencia

### Código del Proyecto
Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

### Dataset
El dataset utilizado está bajo **Creative Commons Attribution 4.0 International (CC BY 4.0)**.



- **Autor**: Matias Caraballo
- **GitHub**: [MatiasCaraballo](https://github.com/MatiasCaraballo)
- **Proyecto**: [prediccion-peliculas](https://github.com/MatiasCaraballo/prediccion-peliculas)
