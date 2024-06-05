# Proyecto final para la Materia Machine Learning

Facilitadora: Dra. Lorena Diaz González.

por: Lizeth Meza Alegria.


Este repositorio contiene dos cuadernos de Jupyter que implementan y analizan modelos de aprendizaje automático para tareas de clasificación y regresión. Los modelos utilizados son Random Forest y GaussianNB para clasificación, y Linear Regression y Decision Tree Regressor para regresión. Además, se ha utilizado GridSearchCV para realizar la búsqueda de hiperparámetros óptimos en cada modelo,excepto en GaussianNB el cual solo cuenta con dos hiperparámetros. A continuación, se presenta una descripción general de cada uno de los cuadernos y los enfoques aplicados en cada tarea.

## Clasificación
### 1. Random Forest Classification:

En esta sección, se implementa un modelo de Random Forest para realizar tareas de clasificación. El Random Forest es un método de aprendizaje automático que construye múltiples árboles de decisión durante el entrenamiento y emite la clase que es el modo de las clases (clasificación) de los árboles individuales.
Se utiliza GridSearchCV para la búsqueda de hiperparámetros óptimos, asegurando que el modelo esté bien ajustado.
El cuaderno incluye un análisis detallado de los hiperparámetros, de los cuales fueron elegidos "criterion", "n_estimators", "max_samples" como los hiperparámetros más relevantes.

### 2. Gaussian Naive Bayes (GaussianNB) Classification:

Esta sección se presenta el modelo GaussianNB, una variante del clasificador Naive Bayes que asume que las características continúan y se distribuyen según una distribución normal (gaussiana).
El modelo GaussianNB tiene menos hiperparámetros en comparación con otros modelos, es por eso que se decide trabajar con los hiperparámetros por defecto sin aplicar el GridSearchCV.

Para ambos modelos se usaron las metricas accuracy, reporte de clasificación y matriz de confusión.

## Regresión
### 1. Linear Regression:

En este cuaderno, se desarrolla un modelo de regresión lineal para predecir valores continuos. La regresión lineal es uno de los métodos más simples y ampliamente utilizados para modelar la relación entre una variable dependiente y una o más variables independientes.
Aunque la regresión lineal tiene pocos hiperparámetros, se emplea GridSearchCV para asegurar que los parámetros disponibles, estén óptimamente ajustados.
Esta sección del cuaderno abarca desde la implementación de la práctica hasta el ajuste del modelo, la interpretación de los coeficientes y la evaluación del rendimiento mediante métricas como el error cuadrático medio (MSE).

### 2. Decision Tree Regressor:

Esta parte explora el uso de árboles de decisión para tareas de regresión. A diferencia de los árboles de decisión utilizados en clasificación, los árboles de decisión para regresión predicen valores continuos dividiendo repetidamente el espacio de características en regiones que minimizan el error en cada partición.
Se emplea GridSearchCV para la búsqueda de hiperparámetros óptimos, tales como la profundidad del árbol y el número mínimo de muestras por hoja, para evitar el sobreajuste.

