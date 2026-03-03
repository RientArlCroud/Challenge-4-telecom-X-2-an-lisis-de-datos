# 📊 Análisis de Cancelación de Clientes – Telecom X  

## 📌 Descripción del Proyecto

Este proyecto tiene como objetivo analizar y predecir la cancelación de clientes (churn) en una empresa ficticia del sector de telecomunicaciones llamada Telecom X.

A través de técnicas de análisis exploratorio de datos y modelos de Machine Learning, se identificaron los principales factores asociados a la cancelación y se evaluaron distintas alternativas predictivas para apoyar la toma de decisiones estratégicas.

El enfoque del proyecto no solo se centró en la construcción de modelos, sino también en la interpretación de resultados y su impacto en el negocio.

## 🎯 Objetivo

Identificar las variables que más influyen en la cancelación de clientes.

Construir y evaluar modelos de clasificación para predecir churn.

Seleccionar el modelo con mejor equilibrio entre detección de clientes en riesgo y control de intervenciones innecesarias.

Proponer estrategias de retención basadas en los resultados obtenidos.

## 📂 Dataset

El conjunto de datos contiene información demográfica, contractual y de servicios de clientes de una empresa de telecomunicaciones, incluyendo:

* Información del contrato

* Tipo de servicio de internet

* Facturación mensual y total

* Tiempo de permanencia

* Variable objetivo: Churn (Sí/No)

## 🛠️ Metodología

El flujo de trabajo seguido fue:

1. Limpieza y preparación de datos.

2. Codificación de variables categóricas mediante One-Hot Encoding.

3. Separación de datos en entrenamiento (70%) y prueba (30%) con estratificación.

4. Estandarización de variables numéricas.

5. Evaluación de modelos mediante:

  * Accuracy

  * Precision

  * Recall

  * F1-score

  * Matriz de confusión

6. Comparación crítica del desempeño de los modelos.

7. Interpretación de variables más influyentes.

## 🤖 Modelos Evaluados

* Dummy Classifier (baseline)

* Regresión Logística

* Regresión Logística con SMOTE

* Random Forest (max_depth = 10)

## 📈 Resultados Principales

- El modelo Dummy demostró que la exactitud por sí sola no es suficiente en problemas desbalanceados.

- La Regresión Logística base mostró el mejor equilibrio entre:

- Sensibilidad en la detección de churn

- Control de falsos positivos

- Estabilidad en la generalización

- Aunque el modelo con SMOTE logró mayor recall, generó un aumento significativo en falsos positivos, lo que implicaría mayores costos operativos en campañas de retención.

- El modelo Random Forest no superó a la Regresión Logística en la métrica clave de sensibilidad.

## 🔎 Factores Clave en la Cancelación

Las variables con mayor impacto en la probabilidad de cancelación fueron:

- Tiempo de permanencia (Tenure)

- Tipo de contrato

- Tipo de servicio de internet

- Estructura de facturación

Se identificó que:

- Clientes con menor permanencia presentan mayor riesgo.

- Contratos mensuales aumentan la probabilidad de cancelación.

- El servicio de fibra óptica mostró mayor asociación con churn.

- Contratos de largo plazo reducen significativamente el riesgo.

## 💡 Conclusiones Estratégicas

* El análisis demuestra que la cancelación puede anticiparse mediante modelos predictivos adecuados.

* La Regresión Logística base fue seleccionada como modelo óptimo por su equilibrio entre precisión y sensibilidad, permitiendo identificar clientes en riesgo sin generar intervenciones excesivas.

* Los resultados permiten diseñar estrategias de retención enfocadas en:

* Incentivar contratos de mayor duración.

* Implementar programas de retención temprana.

* Analizar la experiencia del cliente en el servicio de fibra óptica.

## 🧰 Tecnologías Utilizadas

- Python

- Pandas

- NumPy

- Scikit-learn

- Imbalanced-learn

- Matplotlib

- Google Colab

## 👤 Autor

Proyecto desarrollado por Juan Esteban Rodríguez Aranda  
Ingeniero Ambiental en formación | En transición hacia Ciencia de Datos
