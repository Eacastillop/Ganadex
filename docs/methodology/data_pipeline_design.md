# 🔄 Diseño del Pipeline de Datos

## Descripción
Este documento define la arquitectura y los flujos de procesamiento de datos utilizados en el proyecto de predicción de precios de ganado. Se detallan las etapas clave, las herramientas empleadas y el plan de monitoreo del pipeline.

## 1. Arquitectura del Pipeline de Datos
El pipeline de datos está diseñado para manejar la ingesta, transformación, almacenamiento y disponibilidad de los datos en un entorno escalable basado en AWS. Las fases incluyen:

### 📌 Ingesta de Datos
- **Fuentes de Datos:** Bases de datos históricas, APIs meteorológicas y reportes de mercado.
- **Herramientas:** AWS Glue, Lambda y S3 para extracción y almacenamiento inicial.

### 📌 Transformación y Procesamiento
- **Limpieza de Datos:** Eliminación de valores nulos, outliers y conversión de formatos.
- **Enriquecimiento:** Incorporación de variables adicionales, como clima y tendencias de mercado.
- **Herramientas:** Pandas, PySpark, AWS Glue para ETL.

### 📌 Almacenamiento y Disponibilidad
- **Datos Intermedios:** Almacenados en `data/processed/` en formato Parquet.
- **Datos para Modelado:** Conjunto de datos final listo en `data/validation/`.
- **Herramientas:** Amazon S3, Redshift para almacenamiento estructurado.

## 2. Plan de Monitoreo y Mantenimiento
Para garantizar el correcto funcionamiento del pipeline, se aplican las siguientes estrategias:
- **Monitoreo en tiempo real:** Uso de AWS CloudWatch para seguimiento de errores y rendimiento.
- **Registro de Procesos:** Auditoría con AWS CloudTrail para trazabilidad de cambios.
- **Alertas Automatizadas:** Notificaciones en caso de fallos en la ingesta o procesamiento.

Este pipeline asegura la disponibilidad de datos de alta calidad para el entrenamiento y despliegue del modelo de predicción en AWS SageMaker.

