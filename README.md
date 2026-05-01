# Predicción del Riesgo de Diabetes en Pacientes Adultos

**Proyecto Integrado 3 — Actividad 1**
Institución: IU Digital

---

## Integrantes del Equipo

| Nombre | Correo |
|--------|--------|
| Andrés Mejía | andres.nmejia@mercadolibre.com.co |

---

## I. Definición del Problema de Negocio

### Descripción del Problema

La diabetes mellitus es una enfermedad crónica de alto impacto en los sistemas de salud a nivel mundial. Según la OMS, afecta a más de 422 millones de personas y es una de las principales causas de ceguera, insuficiencia renal, ataques cardíacos y amputaciones. La detección temprana del riesgo de diabetes permite implementar intervenciones preventivas —cambios en el estilo de vida, control de peso, monitoreo de glucosa— que reducen significativamente las complicaciones y los costos asociados a la atención médica.

Este proyecto busca analizar los factores clínicos y demográficos disponibles en el dataset de pacientes adultos del Instituto Nacional de Diabetes y Enfermedades Digestivas y Renales (NIDDK), con el fin de identificar qué variables tienen mayor relación con el diagnóstico positivo de diabetes.

### Pregunta de Investigación

> ¿Cuáles son los factores clínicos con mayor correlación con el diagnóstico de diabetes en pacientes adultos, y con qué precisión se puede caracterizar el perfil de riesgo a partir de variables como glucosa, IMC, edad e historial familiar?

### Métricas de Éxito

- Identificar las **3 a 5 variables** con mayor poder discriminatorio entre pacientes diabéticos y no diabéticos.
- Obtener un **perfil de datos completo** que documente la distribución, valores nulos, outliers y correlaciones del dataset.
- Producir un reporte de exploración (Pandas Profiling) que sirva como base sólida para futuras etapas de modelado predictivo.
- Documentar hallazgos y conclusiones accionables sobre la calidad del dataset y las variables de interés.

---

## II. Fuente de Datos

| Atributo | Detalle |
|----------|---------|
| **Nombre** | Pima Indians Diabetes Database |
| **Fuente** | Kaggle / UCI ML Repository |
| **Origen** | National Institute of Diabetes and Digestive and Kidney Diseases (NIDDK) |
| **Formato** | CSV |
| **Registros** | 768 filas |
| **Variables** | 9 columnas |

### Variables del Dataset

| Variable | Descripción | Tipo |
|----------|-------------|------|
| `Pregnancies` | Número de embarazos | Numérica |
| `Glucose` | Concentración de glucosa en plasma (2h test oral) | Numérica |
| `BloodPressure` | Presión arterial diastólica (mm Hg) | Numérica |
| `SkinThickness` | Grosor del pliegue cutáneo (mm) | Numérica |
| `Insulin` | Insulina sérica 2h (mu U/ml) | Numérica |
| `BMI` | Índice de masa corporal (kg/m²) | Numérica |
| `DiabetesPedigreeFunction` | Función de historial familiar de diabetes | Numérica |
| `Age` | Edad en años | Numérica |
| `Outcome` | Diagnóstico (1 = diabético, 0 = no diabético) | Binaria |

---

## Estructura del Repositorio

```
Actividad1/
├── README.md
├── data/
│   └── diabetes.csv          # Dataset (descargar de Kaggle)
├── notebooks/
│   └── exploracion.ipynb     # EDA con Pandas Profiling
└── .gitignore
```

---

## Cómo Ejecutar

1. Descargar `diabetes.csv` desde [Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) y colocarlo en `data/`.
2. Instalar dependencias:
   ```bash
   pip install pandas ydata-profiling notebook
   ```
3. Abrir y ejecutar el notebook:
   ```bash
   jupyter notebook notebooks/exploracion.ipynb
   ```
