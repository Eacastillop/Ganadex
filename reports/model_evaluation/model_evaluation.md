# 🔎 Evaluación de Modelos

## Descripción
Este documento detalla el desempeño de los modelos de predicción de precios de ganado utilizados en el proyecto. Se incluyen métricas de evaluación, comparación entre modelos y justificación de la elección final.

## 1. Modelos Evaluados
Se probaron diferentes algoritmos de machine learning para determinar cuál ofrecía la mejor precisión en la predicción de precios:
- **Random Forest**
- **XGBoost**
- **Regresión Lineal** (como modelo base para comparación)

## 2. Métricas de Evaluación
| **Métrica** | **Random Forest** | **XGBoost** | **Regresión Lineal** |
|------------|-----------------|------------|------------------|
| RMSE (Error Cuadrático Medio) | 191.17 | **187.59** | 230.45 |
| R² (Coeficiente de Determinación) | 0.77 | **0.78** | 0.65 |
| MAE (Error Absoluto Medio) | 140.25 | **135.30** | 175.40 |

## 3. Comparación y Justificación de la Elección
- **XGBoost obtuvo el mejor desempeño general**, con el menor error (RMSE de 187.59) y el mayor R² (0.78), indicando una mejor capacidad predictiva.
- **Random Forest** mostró un desempeño similar, pero con un RMSE ligeramente mayor.
- **La Regresión Lineal no capturó adecuadamente la complejidad de los datos**, con un R² más bajo y mayor error.

Dado que **XGBoost minimiza el error de predicción y generaliza mejor en distintos conjuntos de datos**, fue seleccionado como el modelo final para su despliegue en producción.

## 4. Validación del Modelo
Para garantizar la confiabilidad del modelo, se aplicaron las siguientes estrategias:
- **Validación Cruzada:** Evaluación en diferentes particiones del dataset para evitar sobreajuste.
- **Pruebas en Datos No Vistos:** Se validó el modelo en un conjunto de datos separado para comprobar su capacidad de generalización.
- **Monitoreo en Producción:** Implementación de AWS CloudWatch para detectar posibles desviaciones en las predicciones.

## 5. Conclusión
El modelo final basado en **XGBoost** proporciona predicciones precisas y confiables para la estimación de precios de ganado. Su implementación en **AWS SageMaker** permite consultas en tiempo real, optimizando la toma de decisiones del sector agropecuario.

