# 📊 Descripción de los Datos

## Descripción
Este documento proporciona información detallada sobre los datos utilizados en el proyecto de predicción de precios de ganado, incluyendo su estructura, fuentes y uso dentro del pipeline de datos.

## 1. Estructura de los Datos
El dataset principal contiene registros históricos de precios de ganado junto con variables adicionales que influyen en las fluctuaciones del mercado.

| **Variable**         | **Descripción**                                | **Tipo**    |
|----------------------|----------------------------------------------|------------|
| `fecha`             | Fecha de la transacción                      | Date       |
| `categoria`         | Categoría del ganado (ternero, vaca, toro)   | Categórica |
| `peso_kg`           | Peso promedio del ganado en kilogramos       | Numérica   |
| `precio_kg`        | Precio del ganado por kilogramo en USD       | Numérica   |
| `ubicacion`         | Región donde se realizó la transacción       | Categórica |
| `temperatura`       | Temperatura media en la fecha de la venta    | Numérica   |
| `precipitacion_mm`  | Nivel de precipitación en la región          | Numérica   |
| `demanda_mercado`   | Índice de demanda basado en datos históricos | Numérica   |

## 2. Fuentes de Datos
Los datos provienen de diversas fuentes para garantizar precisión y confiabilidad:
- **Bases de datos de mercados ganaderos**: Registros de precios históricos y transacciones.
- **APIs climáticas**: Información meteorológica histórica y actual.
- **Reportes económicos del sector agropecuario**: Datos sobre oferta y demanda.

## 3. Uso de los Datos en el Proyecto
- **Entrenamiento del Modelo**: Se utilizan variables relevantes para predecir el precio del ganado por kilogramo.
- **Validación y Evaluación**: Se separa un conjunto de datos para medir el desempeño del modelo.
- **Despliegue y Predicción en Tiempo Real**: Los datos recientes se ingresan al modelo para obtener predicciones actualizadas.

## 4. Consideraciones de Calidad
Para garantizar la calidad de los datos:
- Se realiza **detección y eliminación de valores atípicos**.
- Se aplican **técnicas de imputación** para datos faltantes.
- Se validan los datos con fuentes cruzadas para evitar inconsistencias.

Este documento debe actualizarse conforme se incorporen nuevas variables o fuentes de datos al proyecto.

