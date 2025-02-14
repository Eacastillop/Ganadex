# ⚠️ Evaluación de Riesgos

## Descripción
Este documento identifica los posibles riesgos que podrían afectar el éxito del proyecto de predicción de precios de ganado. Se presentan estrategias de mitigación para minimizar su impacto.

## 1. Identificación de Riesgos
| **Riesgo** | **Descripción** | **Impacto** | **Probabilidad** |
|------------|----------------|-------------|------------------|
| Datos insuficientes o de baja calidad | Falta de registros históricos completos o inconsistencias en los datos. | Alto | Medio |
| Sobrecoste en AWS SageMaker | Costos mayores a los estimados debido a uso ineficiente de recursos en la nube. | Medio | Alto |
| Errores en el modelo de predicción | Bajo rendimiento del modelo debido a datos mal procesados o sobreajuste. | Alto | Medio |
| Fallos en el despliegue del endpoint | Problemas técnicos en la implementación del modelo en producción. | Alto | Bajo |
| Seguridad de los datos | Posibles accesos no autorizados o pérdida de información. | Alto | Bajo |

## 2. Plan de Mitigación
| **Riesgo** | **Estrategia de Mitigación** |
|------------|---------------------------|
| Datos insuficientes o de baja calidad | Implementar validaciones y limpieza de datos antes del modelado. Incorporar fuentes de datos externas si es necesario. |
| Sobrecoste en AWS SageMaker | Optimizar instancias y monitorear uso con AWS CloudWatch. Evaluar modelos más eficientes en consumo de recursos. |
| Errores en el modelo de predicción | Aplicar técnicas de validación cruzada y ajustar hiperparámetros. Evaluar diferentes algoritmos y métricas. |
| Fallos en el despliegue del endpoint | Realizar pruebas en entornos de staging antes de la producción. Configurar alertas para fallos en AWS. |
| Seguridad de los datos | Aplicar cifrado en tránsito y en reposo. Control de acceso con AWS IAM y auditorías con AWS CloudTrail. |

Este análisis permite anticipar y minimizar los riesgos, asegurando la estabilidad y éxito del proyecto.

