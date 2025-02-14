# 🧹 Calidad de Datos

## Descripción
Este informe analiza la calidad de los datos utilizados en el proyecto de predicción de precios de ganado. Se identifican problemas en la fuente de datos, estrategias de limpieza y métodos aplicados para mejorar su calidad.

## 1. Análisis de Calidad de Datos
Para garantizar la fiabilidad del modelo, se evaluaron los siguientes aspectos:
- **Valores nulos y faltantes:** Datos incompletos en variables clave como temperatura y categoría de ganado.
- **Inconsistencias en valores:** Diferencias en unidades de medida y formatos incorrectos en precios.
- **Sesgo en datos:** Variaciones estacionales que pueden afectar la predicción.
- **Valores atípicos:** Precios anormalmente altos o bajos que podrían distorsionar el modelo.

## 2. Estrategias de Limpieza de Datos
Se aplicaron los siguientes métodos para mejorar la calidad del dataset:
- **Imputación de valores faltantes:** Uso de interpolación y medias móviles para completar datos climáticos.
- **Conversión de formatos:** Estandarización de unidades y normalización de precios.
- **Eliminación de outliers:** Detección mediante percentiles y z-score para remover datos extremos.
- **Revisión de duplicados:** Eliminación de registros redundantes que podrían sesgar el modelo.

## 3. Evaluación de la Calidad Final
Después del preprocesamiento, se verificaron los siguientes aspectos:
- **Distribución uniforme de datos tras limpieza.**
- **Reducción de valores nulos a menos del 1%.**
- **Mantenimiento de la varianza original sin eliminar información clave.**

Este proceso asegura que los datos sean adecuados para entrenar el modelo de predicción con un alto nivel de precisión y confiabilidad.

