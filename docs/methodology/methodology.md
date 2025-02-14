# 📜 Justificación de la Metodología

## Descripción
Este documento explica la metodología utilizada para la ejecución del proyecto de predicción de precios de ganado. Se realiza una comparación entre metodologías aplicables y se justifica la elección de TDSP como marco de trabajo.

## 1. Comparación de Metodologías
A continuación, se comparan tres metodologías comúnmente utilizadas en proyectos de ciencia de datos:

| Criterio        | TDSP (Team Data Science Process) | CRISP-DM (Cross Industry Standard Process for Data Mining) | KDD (Knowledge Discovery in Databases) |
|----------------|---------------------------------|-----------------------------------------------|-----------------------------------|
| **Foco**      | Ciclo de vida completo del ML con énfasis en despliegue | Enfoque estructurado para minería de datos | Proceso de descubrimiento de conocimiento en bases de datos |
| **Iteración** | Sí, con enfoque en mejora continua | Sí, basado en seis fases iterativas | No es iterativo, sigue un flujo secuencial |
| **Despliegue** | Considerado desde el inicio con integración en producción | No es prioridad, centrado en análisis exploratorio | No contempla el despliegue del modelo |
| **Colaboración** | Diseñado para trabajo en equipo con repositorios compartidos | No enfatiza la colaboración entre equipos | Enfocado en descubrimiento de patrones |

## 2. Justificación de TDSP
La metodología **TDSP** fue seleccionada para este proyecto debido a las siguientes razones:
- **Enfoque en ciclo de vida completo:** Abarca desde la ingesta de datos hasta el despliegue del modelo en AWS SageMaker.
- **Estructura modular y colaborativa:** Facilita la organización del trabajo entre equipos de ciencia de datos, ingeniería de datos y operaciones.
- **Orientado a despliegue en producción:** Permite integrar el modelo con sistemas empresariales mediante endpoints en la nube.
- **Iteración y mejora continua:** Se pueden realizar ajustes basados en nuevas fuentes de datos y retroalimentación del negocio.

Esta metodología garantiza un flujo de trabajo estructurado, asegurando que los datos sean gestionados de manera efectiva y que el modelo de predicción pueda ser utilizado en un entorno real de toma de decisiones.

