# Predicción de Churn y Segmentación Inteligente de Usuarios mediante Machine Learning

## Descripción

Este proyecto desarrolla una solución analítica orientada a la identificación de usuarios con riesgo de abandono (Churn) mediante técnicas de Ciencia de Datos y Machine Learning.

La solución integra procesos de ingeniería de datos, análisis exploratorio, modelado predictivo y segmentación de clientes, utilizando Databricks como plataforma de procesamiento, PyCaret y Scikit-learn para el entrenamiento de modelos y Power BI para la construcción del dashboard ejecutivo.

---

# Objetivo General

Desarrollar un modelo de Machine Learning capaz de identificar usuarios con riesgo de abandono y posteriormente segmentarlos mediante el algoritmo K-Means para apoyar la toma de decisiones estratégicas relacionadas con campañas de retención, recuperación y fidelización.

---

# Tecnologías utilizadas

- Python
- Databricks
- PySpark
- Pandas
- NumPy
- Scikit-learn
- PyCaret
- MySQL
- Power BI

---

# Arquitectura del proyecto

```text
Fuente de datos
       │
       ▼
     MySQL
       │
       ▼
Databricks (Lakehouse)
       │
       ├── Preparación de datos
       ├── Feature Engineering
       ├── Modelo Predictivo
       ├── Segmentación K-Means
       │
       ▼
Power BI
       │
       ▼
Dashboard Ejecutivo
```---

# Flujo del proyecto

El proyecto fue desarrollado siguiendo las siguientes etapas:

1. **Creación de la base de datos** en MySQL.
2. **Carga de datos** y preparación del entorno en Databricks.
3. **Análisis Exploratorio de Datos (EDA)** para comprender el comportamiento de las variables.
4. **Feature Engineering**, donde se construyeron las variables más relevantes para el modelo.
5. **Entrenamiento del modelo predictivo** utilizando PyCaret para identificar usuarios con riesgo de abandono (Churn).
6. **Segmentación de usuarios críticos** mediante el algoritmo K-Means implementado con Scikit-learn.
7. **Construcción del Dashboard Ejecutivo** en Power BI para facilitar el análisis y la toma de decisiones.

---

# Notebooks desarrollados

| Notebook | Descripción |
|----------|-------------|
| 01_setup_schema | Creación de la base de datos y definición del esquema. |
| 02_insercion_datos | Carga e inserción de los datos en la base de datos. |
| 03_eda_exploratorio | Análisis exploratorio de datos y comprensión del comportamiento de los usuarios. |
| 04_feature_engineering | Construcción de variables para el modelo de Machine Learning. |
| 05_modelo_ML | Entrenamiento y evaluación del modelo predictivo utilizando PyCaret. |
| 06_vista_powerbi | Generación de la vista utilizada por Power BI para la construcción de los dashboards. |

---

# Dashboard Ejecutivo

El dashboard fue desarrollado en Power BI con el objetivo de facilitar la interpretación del modelo de Machine Learning y apoyar la toma de decisiones del negocio.

Los dashboards permiten analizar el comportamiento de los usuarios, identificar patrones de abandono y segmentar los clientes críticos mediante K-Means.

## 1. Resumen Ejecutivo

![Resumen Ejecutivo](images/Dashboard_resumen_ejecutivo.png)

## 2. Comportamiento de Usuarios

![Comportamiento Usuarios](images/Dashboard_comportamiento_usuarios.png)

## 3. Análisis de Recencia y Frecuencia

![Recencia Frecuencia](images/Dashboard_analisis_recencia_frecuencia.png)

## 4. Análisis de Preferencias

![Preferencias](images/Dashboard_analisis_preferencia.png)

## 5. Campañas de Retención y Acciones Recomendadas

![Campañas](images/Dashboard_campanas_acciones_recomendadas.png)

## 6. Determinación de Clústeres

![Clústeres](images/Dashboard_determinacion_clusteres.png)

---

# Modelo Relacional

![Modelo Relacional](images/Modelo_Relacional_Prediccion_Usuarios_Ausentes.png)
---

# Resultados obtenidos

La solución permitió identificar los usuarios con mayor probabilidad de abandono mediante un modelo predictivo de Machine Learning.

Posteriormente, los usuarios críticos fueron segmentados mediante el algoritmo K-Means, obteniendo cuatro perfiles con características claramente diferenciadas:

- **Clúster 0:** Usuarios recientes con alto riesgo.
- **Clúster 1:** Clientes en abandono avanzado.
- **Clúster 2:** Clientes con alto potencial de recuperación.
- **Clúster 3:** Clientes con actividad histórica moderada.

La segmentación permitió diseñar estrategias específicas para cada perfil, facilitando la toma de decisiones del área de negocio y optimizando las campañas de retención y recuperación de clientes.

---

# Variables utilizadas para el modelo

El modelo de Machine Learning fue construido utilizando variables relacionadas con el comportamiento histórico del usuario, entre ellas:

- Días desde la última apuesta.
- Antigüedad del cliente.
- Número total de apuestas.
- Tendencia de frecuencia.
- Monto total depositado.
- Monto promedio apostado.
- Tasa de pérdida.
- Días sin apuestas.
- Días sin depósitos.

Estas variables fueron sometidas a un proceso de **Feature Engineering**, permitiendo mejorar el desempeño del modelo y la calidad de la segmentación.
---

# Conclusiones

- Se desarrolló una solución integral para la identificación y segmentación de usuarios con riesgo de abandono utilizando técnicas de Ciencia de Datos y Machine Learning.

- La implementación de PyCaret permitió construir un modelo predictivo de manera eficiente, mientras que el algoritmo K-Means facilitó la identificación de cuatro perfiles de usuarios con comportamientos similares.

- La integración de Databricks, MySQL y Power BI permitió construir un flujo completo de datos, desde la preparación de la información hasta la generación de dashboards ejecutivos para apoyar la toma de decisiones.

- Los resultados obtenidos permiten diseñar estrategias diferenciadas de retención, recuperación y fidelización, incrementando el valor de negocio de la solución desarrollada.

---

# Autor

**Deyanira Jaramillo**

Proyecto desarrollado como práctica de Ciencia de Datos, Machine Learning y Business Intelligence utilizando Databricks, PyCaret, Scikit-learn y Power BI.