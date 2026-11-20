# Implementación de mecanismos de atención y Transformers para series de tiempo

## Descripción

Este proyecto desarrolla dos implementaciones de modelos de aprendizaje profundo aplicados al análisis y predicción de series de tiempo. Se implementa un mecanismo de atención y una arquitectura Transformer básica utilizando Python, TensorFlow y Keras.

El propósito es comprender el funcionamiento de estos modelos, evaluar su desempeño y comparar sus resultados mediante métricas de error.

## Objetivo

Implementar y analizar mecanismos de atención y arquitecturas Transformer para realizar predicciones sobre una serie de tiempo, identificando sus características y diferencias en el desempeño.

## Tecnologías utilizadas

- Python
- Google Colab
- TensorFlow y Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Desarrollo

### 1. Mecanismo de atención

Se implementó un mecanismo de atención que asigna diferentes pesos a los pasos temporales de entrada para generar una representación ponderada y realizar la predicción del siguiente valor.

### 2. Arquitectura Transformer

Se desarrolló un Transformer Encoder simplificado que incorpora codificación posicional, atención multicabeza (*Multi-Head Attention*), redes feed-forward, conexiones residuales y normalización.

### Preparación de datos

Se utilizó una serie de tiempo sintética de 1500 registros, compuesta por tendencia, componentes estacionales y ruido aleatorio. Se construyeron ventanas de 30 pasos temporales para predecir el siguiente valor.

Los datos se dividieron cronológicamente en conjuntos de entrenamiento y prueba, y se aplicó normalización mediante MinMaxScaler.

## Resultados

Los modelos se evaluaron mediante las métricas MAE y RMSE.

| Modelo | MAE | RMSE |
|---|---:|---:|
| Mecanismo de atención | 0.665713 | 0.775770 |
| Transformer | 0.671686 | 0.772586 |

El mecanismo de atención obtuvo un MAE ligeramente menor, mientras que el Transformer presentó un RMSE ligeramente inferior. Los resultados muestran un desempeño similar entre ambas implementaciones, sin una ventaja concluyente de un modelo sobre el otro.

## Conclusión

La práctica permitió comprender e implementar dos enfoques basados en mecanismos de atención para el análisis de series de tiempo. Se observó que las arquitecturas Transformer permiten incorporar atención multicabeza y codificación posicional, aunque una mayor complejidad arquitectónica no garantiza necesariamente mejores resultados en todas las métricas.

## Autor

Yohan Steven Dussan Alzate
