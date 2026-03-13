# 📊 Fundamentos de Datos

## Descripción del Curso

Curso práctico de fundamentos de datos con Python, orientado al análisis de **datos hídricos y ambientales**. A lo largo de 4 semanas, el estudiante aprenderá desde la carga y visualización de datos hasta la construcción de modelos de regresión lineal, pasando por limpieza, transformación e ingeniería de características.

**Dataset principal:** Datos de calidad del agua (Water Quality Dataset) — incluye variables fisicoquímicas como pH, dureza, sólidos disueltos, cloraminas, sulfatos, conductividad, carbono orgánico, trihalometanos, turbidez y potabilidad del agua.

---

## 🗓️ Plan por Semanas

### Week 1 — Carga de Datos y Visualización Básica

**Notebook:** `01_carga_datos_visualizacion.ipynb`

| Tema | Contenido |
|------|-----------|
| **Carga desde CSV** | `pd.read_csv()` con archivos locales, manejo de separadores, encoding y parámetros comunes |
| **Carga desde Excel** | `pd.read_excel()` con hojas específicas y rangos |
| **Carga desde la nube (GitHub)** | Lectura directa usando URL raw de un repositorio de GitHub |
| **Carga desde Google Sheets** | Lectura usando enlace público exportado como CSV |
| **Exploración inicial** | `.head()`, `.info()`, `.describe()`, `.shape`, `.dtypes`, `.columns` |
| **Visualización con Matplotlib** | Histogramas, gráficos de barras, scatter plots, personalización de ejes y títulos |
| **Visualización con Seaborn** | Heatmaps de correlación, boxplots, pairplots, violin plots |
| **Visualización con Plotly Express** | Gráficos interactivos: scatter, bar, histogram, box con hover y color |

---

### Week 2 — Calidad, Limpieza, Transformación e Ingeniería de Datos

**Notebook:** `02_calidad_limpieza_transformacion.ipynb`

| Sección | Tema | Contenido |
|---------|------|-----------|
| **1** | **Fundamentos de la Calidad de Datos** | |
| 1.1 | Introducción a la Calidad de Datos | Importancia de datos limpios y confiables para el análisis y la toma de decisiones |
| 1.2 | Dimensiones Clave de la Calidad | Exactitud, Completitud, Consistencia, Validez, Unicidad |
| 1.3 | Diagnóstico de Problemas | Técnicas y herramientas para identificar problemas comunes de calidad |
| **2** | **Técnicas de Limpieza de Datos** | |
| 2.1 | Manejo de Valores Faltantes | Identificación de NaN/None, eliminación vs. imputación (media, mediana, moda, constantes) |
| 2.2 | Tratamiento de Datos Duplicados | Detección y eliminación de registros idénticos |
| 2.3 | Detección y Manejo de Outliers | Métodos IQR y Z-score; estrategias de eliminación, transformación e imputación |
| **3** | **Transformación y Preprocesamiento** | |
| 3.1 | Normalización y Estandarización | Escalado Min-Max [0,1] y Puntuación Z (media=0, std=1) |
| 3.2 | Codificación de Variables Categóricas | Label Encoding (ordinales) y One-Hot Encoding (nominales) |
| 3.3 | Discretización (Binning) | Agrupación de valores numéricos en intervalos |
| **4** | **Ingeniería de Características** | |
| 4.1 | Creación de Nuevas Variables | Generación de características informativas a partir de las existentes |
| 4.2 | Extracción de Características | Derivación de información de datos complejos (fechas, texto) |
| **5** | **Aplicación Práctica con Pandas** | |
| 5.1 | Manipulación Avanzada | `apply()`, `map()`, `transform()`, `groupby()`, merge/join/concat |

---

### Week 3 — Análisis Estadístico y Formulación de Hipótesis

**Notebook:** `03_correlacion_hipotesis.ipynb`

| Tema | Contenido |
|------|-----------|
| **Correlación** | Coeficiente de Pearson, Spearman y Kendall; matrices de correlación; interpretación visual con heatmaps |
| **Homoscedasticidad** | Definición, importancia como supuesto estadístico, pruebas (Breusch-Pagan, Goldfeld-Quandt), interpretación gráfica de residuos |
| **Heteroscedasticidad** | Identificación, consecuencias en modelos de regresión, estrategias de corrección (transformaciones, WLS) |
| **Multicolinealidad** | Definición, detección mediante VIF (Factor de Inflación de Varianza) y matrices de correlación, efectos en regresión |
| **Pregunta de investigación** | Formulación de una pregunta clara y medible a partir de los datos ambientales/hídricos |
| **Hipótesis** | Construcción de hipótesis nula (H₀) y alternativa (H₁), pruebas de hipótesis (t-test, ANOVA), significancia estadística (p-valor) |

---

### Week 4 — Regresión Lineal Simple y Múltiple

**Notebook:** `04_regresion_lineal.ipynb`

| Tema | Contenido |
|------|-----------|
| **Fundamentos de Regresión** | Concepto, supuestos, ecuación de la recta, función de costo (MSE) |
| **Regresión Lineal Simple** | Implementación con scikit-learn, ajuste del modelo, predicciones, visualización de la recta de regresión |
| **Evaluación del Modelo Simple** | R², MSE, RMSE, MAE, interpretación de coeficientes |
| **Regresión Lineal Múltiple** | Extensión a múltiples variables predictoras, selección de features, ajuste e interpretación |
| **Evaluación del Modelo Múltiple** | Comparación de métricas, R² ajustado, análisis de residuos |
| **Validación de Supuestos** | Normalidad de residuos, linealidad, independencia, homoscedasticidad (aplicación de Week 3) |
| **Caso Práctico Completo** | Pipeline completo: desde la carga y limpieza hasta el modelo final con datos de calidad del agua |

---

## 🛠️ Tecnologías y Librerías

| Librería | Uso |
|----------|-----|
| `pandas` | Manipulación y análisis de datos |
| `numpy` | Operaciones numéricas |
| `matplotlib` | Visualización estática |
| `seaborn` | Visualización estadística |
| `plotly` | Visualización interactiva |
| `scikit-learn` | Modelos de ML, preprocesamiento, métricas |
| `scipy` | Pruebas estadísticas |
| `statsmodels` | Diagnóstico de regresión, pruebas de heteroscedasticidad |

## 📂 Estructura del Repositorio

```
material-fundamentos_datos/
├── README.md
├── Week_1/
│   └── 01_carga_datos_visualizacion.ipynb
├── Week_2/
│   └── 02_calidad_limpieza_transformacion.ipynb
├── Week_3/
│   └── 03_correlacion_hipotesis.ipynb
└── Week_4/
    └── 04_regresion_lineal.ipynb
```

## 📊 Dataset

Se utilizará el **Water Quality Dataset** a lo largo de todas las semanas, el cual contiene mediciones fisicoquímicas del agua:

| Variable | Descripción |
|----------|-------------|
| `ph` | Nivel de pH del agua |
| `Hardness` | Dureza del agua (mg/L) |
| `Solids` | Sólidos disueltos totales (ppm) |
| `Chloramines` | Cantidad de cloraminas (ppm) |
| `Sulfate` | Cantidad de sulfatos (mg/L) |
| `Conductivity` | Conductividad eléctrica (μS/cm) |
| `Organic_carbon` | Carbono orgánico (ppm) |
| `Trihalomethanes` | Trihalometanos (μg/L) |
| `Turbidity` | Turbidez (NTU) |
| `Potability` | Potabilidad (1 = potable, 0 = no potable) |

> Este dataset permite explorar relaciones entre variables ambientales, detectar patrones de calidad del agua y construir modelos predictivos de potabilidad.

---

## 📝 Licencia

Material académico de uso educativo.
