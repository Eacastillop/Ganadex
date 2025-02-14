# 🔧 Guía de Estilo y Buenas Prácticas de Código

## Descripción
Este documento establece las mejores prácticas y lineamientos para el desarrollo y mantenimiento del código en el proyecto de predicción de precios de ganado. Se busca garantizar la claridad, reutilización y eficiencia del código.

## 1. Estructura del Código
El código debe estar modularizado en funciones y clases reutilizables para facilitar el mantenimiento y la escalabilidad.
- **`preprocessing/`** → Scripts para limpieza y transformación de datos.
- **`modeling/`** → Scripts para entrenamiento y evaluación de modelos.
- **`deployment/`** → Scripts para despliegue del modelo en producción.
- **`utils/`** → Funciones auxiliares reutilizables en diferentes módulos.

## 2. Estándares de Codificación
### 📌 Estilo de Código
- Seguir el estándar **PEP 8** para código en Python.
- Nombres de variables y funciones en **snake_case**.
- Nombres de clases en **PascalCase**.
- Mantener líneas de código con un máximo de **79 caracteres**.

### 📌 Documentación
- Cada función y clase debe incluir una docstring con su propósito, parámetros y retorno.
```python
def calcular_rmse(y_real, y_pred):
    """
    Calcula el Error Cuadrático Medio (RMSE) entre los valores reales y predichos.
    
    Parámetros:
    y_real (array): Valores reales.
    y_pred (array): Valores predichos.
    
    Retorna:
    float: RMSE calculado.
    """
    return np.sqrt(mean_squared_error(y_real, y_pred))
```

### 📌 Manejo de Errores
- Implementar bloques **try-except** para captura y manejo adecuado de errores.
- Usar logging en lugar de prints para mejor trazabilidad de errores.
```python
import logging
logging.basicConfig(level=logging.INFO)

try:
    resultado = dividir(10, 0)
except ZeroDivisionError as e:
    logging.error(f"Error en la función dividir: {e}")
```

## 3. Versionado y Control de Código
- Utilizar **Git** para el control de versiones.
- Seguir la convención de commits semánticos (`feat:`, `fix:`, `refactor:`).
- Mantener ramas separadas para desarrollo y producción (`main`, `dev`).

## 4. Pruebas y Validación
- Implementar pruebas unitarias con **pytest** para validar funciones críticas.
- Automatizar pruebas en CI/CD antes del despliegue en producción.

## 5. Buenas Prácticas en Colaboración
- Realizar revisiones de código mediante **pull requests** en GitHub.
- Escribir código claro y comentado para facilitar la colaboración entre equipos.
- Mantener un archivo `requirements.txt` con las dependencias del proyecto.

Aplicando estas buenas prácticas, garantizamos un código mantenible, eficiente y listo para la implementación en AWS SageMaker.

