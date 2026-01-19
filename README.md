# Student-Performance-Analytics
Pipeline de limpieza de datos y análisis exploratorio para identificar factores de éxito académico.

# 🎓 Análisis de Rendimiento Estudiantil (EDA & Data Cleaning)

> *"Transformando datos crudos en insights educativos para reducir la deserción académica."*

Este proyecto se centra en la etapa más crítica de cualquier proyecto de Ciencia de Datos: la **Ingeniería y Limpieza de Datos (Data Wrangling)**. Utilizando un dataset real de Kaggle, se construyó un pipeline en Python para depurar la información, tratar inconsistencias y revelar los patrones ocultos que determinan el éxito o fracaso de un estudiante.

## 🎯 Objetivo del Proyecto
El análisis busca responder preguntas clave para las instituciones educativas mediante la evidencia estadística:
1.  **Calidad del Dato:** Garantizar la integridad de la información tratando valores nulos y atípicos (outliers).
2.  **Identificación de Patrones:** ¿Influye más la cantidad de horas de estudio o la metodología?
3.  **Visualización Estratégica:** Crear tableros que permitan detectar alumnos en riesgo de reprobación.

**📂 Fuente de Datos:** [Kaggle - Student Academic Performance Dataset](https://www.kaggle.com/datasets/prince7489/student-academic-performance-dataset)

---

## 🔍 Data Storytelling: Insights Revelados
Más allá de limpiar tablas, el objetivo es interpretar el comportamiento estudiantil.

### 1. El Mito de las "Horas Silla"
> ![Correlación de Variables](heatmap_estudiante.png)
>
> * **El Hallazgo:** El análisis de correlación desmiente la idea tradicional de que "más horas sentado estudiando" garantizan el éxito. La correlación entre *Horas de Estudio* y *Rendimiento* es positiva pero moderada.
> * **Traducción:** La **calidad y el método** de estudio son predictores más fuertes que la simple cantidad de tiempo invertido.

### 2. El Debate: ¿Online vs. Híbrido?
> ![Rendimiento por Método](boxplot_estudiante.png)
>
> * **Análisis Comparativo:** Al segmentar la data, observamos que los estudiantes con metodología **"Mixed" (Híbrida)** presentan una mediana de notas superior y, lo más importante, una menor dispersión en el bajo rendimiento comparado con el formato 100% Online.

### 3. Radiografía del Riesgo Académico
> ![Distribución de Notas](histograma_estudiante.png)
>
> * **Diagnóstico:** La distribución de notas sigue una curva normal con un ligero sesgo positivo. Sin embargo, la "cola izquierda" del gráfico permite identificar y aislar al segmento de **Alumnos en Riesgo Crítico** para intervenciones tempranas.

---

## 🛠️ Ingeniería de Datos (Pipeline Técnico)
El valor central de este repositorio es la demostración de habilidades sólidas en manipulación de datos con **Pandas**.

### 1. Limpieza y Tratamiento (Data Cleaning)
* **Archivo:** `TF4_G01.ipynb`
* **Manejo de Nulos:** Implementación de estrategias de imputación (media/moda) para no perder registros valiosos.
* **Detección de Outliers:** Uso del Rango Intercuartil (IQR) para identificar anomalías en las horas de estudio y uso de dispositivos.
* **Normalización:** Estandarización de escalas de calificación (0-20) para análisis comparativos.

### 2. Feature Engineering
* **Categorización:** Transformación de variables continuas en categorías de negocio (ej. "Aprobado/Desaprobado", "Alto Rendimiento").
* **Creación de KPIs:** Generación de nuevas métricas derivadas para enriquecer el análisis.

## 📦 Stack Tecnológico
* **Lenguaje:** Python 3.x
* **Manipulación:** `Pandas`, `NumPy`.
* **Visualización:** `Seaborn`, `Matplotlib`.
* **Formato:** Procesamiento de `CSV` y exportación de reportes limpios.

---
*Proyecto de Portafolio de Ciencia de Datos | 2026*
