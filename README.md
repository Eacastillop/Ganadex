# 📖 Proyecto de Predicción de Precios de Ganado

## 📌 Contexto del Proyecto
El objetivo principal del proyecto es desarrollar un modelo de machine learning capaz de predecir con precisión el precio por kilogramo de ganado, utilizando datos históricos de transacciones, condiciones climáticas y demanda de mercado. Este modelo será implementado detrás de un endpoint en **Amazon SageMaker**, lo que permitirá realizar predicciones en tiempo real.

## 🚀 Alcance del Proyecto
- **Recopilación y procesamiento de datos históricos de precios de ganado.**
- **Entrenamiento de un modelo de machine learning optimizado para predicción de precios.**
- **Implementación del modelo en AWS SageMaker como un servicio escalable.**
- **Validación y monitoreo del rendimiento del modelo en producción.**

## 🛠️ Tecnologías Utilizadas
- **AWS SageMaker** → Entrenamiento y despliegue del modelo en la nube.
- **AWS S3** → Almacenamiento de datasets procesados.
- **AWS Glue** → Pipeline ETL para transformación de datos.
- **XGBoost / Random Forest** → Algoritmos principales para predicción.
- **Python (Pandas, Scikit-learn, NumPy)** → Análisis y preprocesamiento de datos.
- **FastAPI / Flask** → API alternativa para consultas del modelo.

## 📂 Estructura del Repositorio
```
📦 proyecto-prediccion-ganado
 ├── 📂 data/               # Datos crudos, procesados y de validación
 ├── 📂 notebooks/          # Cuadernos Jupyter para análisis y modelado
 ├── 📂 src/                # Código fuente del modelo y despliegue
 ├── 📂 reports/            # Informes de calidad de datos y evaluación del modelo
 ├── 📂 docs/               # Documentación del proyecto
 ├── README.md              # Descripción del proyecto
```

## 📊 Flujo de Trabajo
1️⃣ **Recolección de Datos** → Se recopilan datos históricos de precios de ganado, condiciones climáticas y demanda de mercado.

2️⃣ **Preprocesamiento** → Se eliminan valores nulos, se normalizan variables y se detectan outliers.

3️⃣ **Entrenamiento del Modelo** → Se prueban diferentes algoritmos (XGBoost, Random Forest) para optimizar la precisión de predicción.

4️⃣ **Evaluación del Modelo** → Se comparan métricas de rendimiento (RMSE, R²) y se selecciona el mejor modelo.

5️⃣ **Despliegue en AWS** → Se configura un endpoint en SageMaker para permitir predicciones en tiempo real.

6️⃣ **Monitoreo y Mejoras** → Se ajusta el modelo según nuevos datos y se optimiza su rendimiento.

## 📬 Contacto
Para dudas o contribuciones, por favor contacta al equipo del proyecto a través de xxx

Este proyecto proporciona una solución automatizada para la predicción de precios de ganado, facilitando decisiones estratégicas en el sector agropecuario. 🚀



## Flujo del proyecto

![mermaid_graph](https://www.mermaidchart.com/raw/fd80f11d-721b-41d3-baa6-6417bad5a430?theme=light&version=v0.1&format=svg)
