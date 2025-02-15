# 👨‍💼 Rol del Project Manager
## Descripción
El **Project Manager** es responsable de la planificación, seguimiento y ejecución del proyecto. Sus responsabilidades incluyen asegurar el cumplimiento de los plazos, mantener comunicación con los stakeholders (en este caso, el cliente) y coordinar reuniones y entregables.

---

## Roles y Responsabilidades

### **1. John - Project Manager**
**Responsabilidades principales:**
- **Planificación y Seguimiento del Proyecto**  
  - Crear y mantener el cronograma del proyecto, asegurando que se cumplan los plazos.
  - Monitorear el progreso de cada fase del proyecto (según CRISP-DM) y ajustar el plan si es necesario.
  - Documentar los avances y riesgos del proyecto.

- **Comunicación con el Cliente**  
  - Mantener comunicación constante con el **cliente** (entidad externa) para asegurar que los entregables cumplan con sus expectativas.
  - Presentar informes de progreso y resultados clave al cliente.
  - Recibir retroalimentación del cliente y ajustar el proyecto según sea necesario.

- **Coordinación del Equipo**  
  - Organizar y liderar reuniones periódicas con el equipo (Jhoan y Edwin) para revisar el avance y resolver problemas.
  - Asignar tareas específicas a cada miembro del equipo y asegurar que se cumplan.
  - Facilitar la colaboración entre Jhoan y Edwin, especialmente en las fases de preprocesamiento y modelado.

**Habilidades clave:**  
- Habilidades de gestión de proyectos y organización.
- Comunicación efectiva con el cliente y el equipo.
- Conocimiento básico de las fases de CRISP-DM y las herramientas de AWS para supervisar el proyecto.

---

### **2. Jhoan - Científico de Datos (Enfoque en Análisis Exploratorio y Preprocesamiento)**
**Responsabilidades principales:**
- **Fase 2: Comprensión de los Datos**  
  - Realizar el análisis exploratorio de datos (EDA) para entender la estructura, calidad y posibles problemas en los datos.
  - Identificar fuentes de datos adicionales para enriquecer el conjunto de datos.
  - Colaborar con Edwin en la limpieza y preparación de los datos.

- **Fase 3: Preparación de los Datos**  
  - Limpiar y transformar los datos: manejo de valores faltantes, normalización, codificación de variables categóricas, etc.
  - Realizar la imputación de datos críticos (por ejemplo, precios del dólar o temperaturas) utilizando técnicas como interpolación o medias móviles.
  - Eliminar valores atípicos y asegurar la calidad de los datos.

**Habilidades clave:**  
- Experiencia en análisis exploratorio de datos (EDA) y preprocesamiento con herramientas como **Python**, **Pandas**, y **AWS Glue**.
- Conocimiento de técnicas de limpieza y transformación de datos.

---

### **3. Edwin - Científico de Datos (Enfoque en Modelado y Evaluación)**
**Responsabilidades principales:**
- **Fase 4: Modelado**  
  - Implementar y entrenar los modelos de machine learning (**XGBoost** y **Random Forest**) en **AWS SageMaker**.
  - Realizar la optimización de hiperparámetros para mejorar la precisión del modelo.
  - Evaluar el rendimiento del modelo utilizando métricas como **RMSE** y **R²**.

- **Fase 5: Evaluación**  
  - Comparar los resultados de los modelos (por ejemplo, XGBoost vs. Random Forest) y seleccionar el mejor modelo basado en las métricas.
  - Realizar pruebas de validación cruzada para asegurar que el modelo generaliza bien.
  - Documentar los resultados y presentar las conclusiones al equipo.

- **Fase 6: Despliegue**  
  - Empaquetar el modelo seleccionado y subirlo a un bucket de **S3**.
  - Configurar el endpoint en **AWS SageMaker** para consultas en tiempo real.
  - Realizar pruebas de inferencia para validar que el modelo funciona correctamente en producción.

**Habilidades clave:**  
- Experiencia en machine learning con algoritmos como **XGBoost** y **Random Forest**.
- Conocimiento de métricas de evaluación de modelos (RMSE, R²).
- Familiaridad con **AWS SageMaker** para entrenamiento y despliegue de modelos.

---

## Colaboración entre Roles
- **John** (Project Manager) será el responsable de la planificación, seguimiento y comunicación con el **cliente**. También coordinará las reuniones y asegurará que los entregables se cumplan a tiempo.
- **Jhoan** se enfocará en el análisis exploratorio de datos y la preparación de los datos, asegurando que estén listos para el modelado.
- **Edwin** se encargará del desarrollo y optimización del modelo, así como de su implementación en producción.

---

## Resumen de Roles

| Rol                     | Responsable | Responsabilidades Clave                                                                 |
|-------------------------|-------------|-----------------------------------------------------------------------------------------|
| **Project Manager**     | John        | Planificación, seguimiento, comunicación con el cliente, coordinación del equipo.       |
| **Científico de Datos (Análisis y Preprocesamiento)** | Jhoan       | Análisis exploratorio de datos, limpieza y transformación de datos.                     |
| **Científico de Datos (Modelado y Evaluación)** | Edwin       | Entrenamiento y optimización de modelos, evaluación, despliegue en AWS SageMaker.       |

---

## Siguientes Pasos
1. **John** (Project Manager) debe crear un cronograma detallado del proyecto, asignar tareas y organizar la primera reunión con el equipo.
2. **Jhoan** debe comenzar con el análisis exploratorio de datos (EDA) y la limpieza de los datos, identificando posibles problemas de calidad.
3. **Edwin** debe definir los algoritmos a utilizar y comenzar con la implementación inicial del modelo en AWS SageMaker.

---

## Cronograma (4 Semanas)

| Fase del Proyecto       | Responsable       | Duración Estimada | Entregables                                                                 |
|-------------------------|-------------------|-------------------|-----------------------------------------------------------------------------|
| **Semana 1: Comprensión del Negocio y Análisis Exploratorio de Datos (EDA)** | John y Jhoan      | 1 semana          | Documento de requisitos y KPIs definidos. Informe de EDA con hallazgos clave. |
| **Semana 2: Preprocesamiento de Datos y Modelado Inicial** | Jhoan y Edwin     | 1 semana          | Conjunto de datos limpio y listo para el modelado. Modelo inicial entrenado. |
| **Semana 3: Optimización del Modelo y Evaluación** | Edwin             | 1 semana          | Modelo optimizado con métricas de evaluación (RMSE, R²).                    |
| **Semana 4: Despliegue y Presentación Final** | John, Jhoan y Edwin | 1 semana          | Endpoint en AWS SageMaker listo para consultas en tiempo real. Presentación de resultados. |
