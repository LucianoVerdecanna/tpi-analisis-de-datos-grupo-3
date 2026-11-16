# Análisis de Churn en una empresa de Telecomunicaciones

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Lea-2005/tpi-analisis-de-datos-grupo-3/blob/main/notebooks/TPI_Analisis_de_Datos.ipynb)

**Trabajo Práctico Integrador — Introducción al Análisis de Datos**
Segundo Parcial · 2º Cuatrimestre · Docente: Enzo Martín Zotti

---

## Problema de negocio

Una empresa de telecomunicaciones pierde clientes que cancelan su servicio (**churn**). Retener a un cliente cuesta mucho menos que conseguir uno nuevo, así que la empresa necesita saber **quiénes cancelan y qué tienen en común** para actuar antes de que se vayan.

En este trabajo analizamos el dataset **Telco Customer Churn** (Kaggle) para:

- Describir el perfil de los clientes que cancelan frente a los que se quedan.
- Medir cómo influyen la antigüedad (`tenure`), el cargo mensual (`MonthlyCharges`), el tipo de contrato y el método de pago en la tasa de cancelación.
- Formular recomendaciones concretas para reducir el churn.

**Variable de interés:** `Churn` (Yes / No).

## Integrantes — Grupo 3 · División 143

| Integrante | GitHub |
|---|---|
| [Nombre Apellido] | [@usuario] |
| [Nombre Apellido] | [@usuario] |
| [Nombre Apellido] | [@usuario] |
| [Nombre Apellido] | [@usuario] |

## Stack tecnológico

| Herramienta | Uso |
|---|---|
| **Python 3** | Lenguaje principal |
| **Google Colab** | Entorno de ejecución reproducible |
| **Pandas** | Ingesta, limpieza y manipulación de datos |
| **NumPy** | Cálculo numérico |
| **Matplotlib** / **Seaborn** | Visualización |
| **SciPy** | Estadística (correlación de Pearson) |
| **Git** / **GitHub** | Control de versiones |

## Estructura del repositorio

```
tpi-analisis-de-datos-grupo-3/
├── README.md                 ← Portada del proyecto (este archivo)
├── requirements.txt          ← Librerías para ejecución local
├── .gitignore
├── data/
│   ├── raw/                  ← Dataset original de Kaggle, sin modificar
│   └── processed/            ← Datos limpios generados por el notebook
├── notebooks/
│   └── TPI_Analisis_de_Datos.ipynb   ← Análisis completo
└── docs/
    └── INFORME_EJECUTIVO.pdf ← Informe con conclusiones de negocio
```

## Cómo explorar el proyecto

**1. Solo leer las conclusiones:** abrí [`docs/INFORME_EJECUTIVO.pdf`](docs/INFORME_EJECUTIVO.pdf).

**2. Ejecutar el análisis en Google Colab (recomendado):**

1. Hacé clic en el badge **Open in Colab** de arriba.
2. En Colab: `Entorno de ejecución → Ejecutar todas`.
3. El notebook carga el dataset directamente desde este repositorio, así que no hace falta subir archivos.

**3. Ejecutar en tu computadora:**

```bash
git clone https://github.com/Lea-2005/tpi-analisis-de-datos-grupo-3.git
cd tpi-analisis-de-datos-grupo-3
pip install -r requirements.txt
jupyter notebook notebooks/TPI_Analisis_de_Datos.ipynb
```

### Recorrido del notebook

| Sección | Contenido |
|---|---|
| **A. Fundamentos, ingesta y limpieza** | Problema e hipótesis, tipos de variables, manipulación con Pandas, nulos, conversión de tipos y outliers |
| **B. Análisis exploratorio y visualización** | Tendencia central, dispersión, correlación de Pearson, tablas de contingencia y reporte gráfico |
| **Conclusiones** | Hallazgos e impacto en el negocio |

## Dataset

- **Fuente:** [Telco Customer Churn — Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Tamaño:** 7.043 clientes × 21 variables
- **Tipo:** datos estructurados (tabla CSV)
- **Ubicación en el repo:** `data/raw/WA_Fn-UseC_-Telco-Customer-Churn.csv`
