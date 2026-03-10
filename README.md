Challenge Telecom X – Parte 2
Predicción de evasión de clientes (Churn) con Machine Learning
Introducción

Este proyecto corresponde a la segunda fase del Challenge Telecom X del programa ONE de Alura Latam, en la cual se da continuidad al análisis realizado en la primera parte del desafío.

Después de completar el análisis exploratorio de datos (EDA) en el primer proyecto, el rol evoluciona de analista de datos a científico de datos, con el objetivo de desarrollar modelos predictivos capaces de anticipar la cancelación de clientes.

Mientras que la primera etapa permitió comprender el pasado y el comportamiento actual de los clientes, esta segunda fase se enfoca en construir herramientas que permitan predecir el futuro, utilizando análisis estadístico y algoritmos de Machine Learning.

El propósito es responder preguntas clave para la empresa Telecom X:

¿Qué clientes tienen mayor riesgo de cancelar el servicio?

¿Qué variables influyen más en este comportamiento?

¿Qué perfiles de clientes requieren mayor atención por parte de la empresa?

Las respuestas a estas preguntas permiten diseñar estrategias de retención más efectivas y personalizadas.

Descripción del proyecto

Este repositorio documenta un proyecto end-to-end de ciencia de datos, cuyo objetivo es analizar y predecir la fuga de clientes (churn) en una empresa de telecomunicaciones.

El proyecto se divide en dos grandes etapas:

Análisis exploratorio de datos (EDA)
Identificación de patrones, comportamientos y factores asociados a la cancelación del servicio.

Modelado predictivo con Machine Learning
Construcción de modelos capaces de estimar la probabilidad de que un cliente abandone la empresa.

El resultado final es un modelo predictivo evaluado con métricas de desempeño, acompañado de un análisis de interpretabilidad que permite comprender las variables más influyentes en las predicciones.

Este enfoque permite transformar datos en información accionable para la toma de decisiones estratégicas.

Objetivos del proyecto
Análisis exploratorio

Identificar el perfil del cliente que cancela el servicio.

Detectar los factores que influyen en la evasión de clientes.

Analizar la relación entre variables demográficas, servicios contratados y comportamiento de cancelación.

Modelado predictivo

Construir un modelo de Machine Learning capaz de predecir la probabilidad de churn.

Evaluar el modelo utilizando métricas relevantes para el negocio, especialmente el recall.

Interpretar el comportamiento del modelo para validar los hallazgos del análisis exploratorio.

Estrategia de negocio

Proporcionar recomendaciones estratégicas basadas en datos.

Proponer acciones concretas para reducir la tasa de cancelación de clientes.

Tecnologías utilizadas

El proyecto fue desarrollado utilizando herramientas ampliamente utilizadas en ciencia de datos y análisis predictivo.

Lenguaje de programación

Python

Análisis y manipulación de datos

Pandas

NumPy

Visualización de datos

Plotly

Matplotlib

Seaborn

Machine Learning

Scikit-learn

Interpretabilidad de modelos

SHAP

Entorno de desarrollo

Google Colab

Metodología de análisis

El proyecto sigue una metodología estructurada basada en el pipeline típico de ciencia de datos.

Fase 1: Análisis Exploratorio de Datos (EDA)
Limpieza y estandarización

Se realizó un proceso exhaustivo de limpieza de datos que incluyó:

Corrección de tipos de datos.

Manejo de valores nulos o inconsistentes.

Estandarización de variables categóricas.

Simplificación de categorías (por ejemplo, unificar valores como "No internet service" en "No").

Visualización de datos

Se utilizaron gráficos interactivos con Plotly para analizar la relación entre cada variable y la variable objetivo Churn.

Se calcularon tasas de cancelación para distintos segmentos de clientes con el fin de identificar patrones relevantes.

Análisis de interacciones

Se analizaron combinaciones de variables que podrían influir en la cancelación, como:

Tipo de contrato y servicio de internet.

Antigüedad del cliente y cargos mensuales.

Servicios adicionales y comportamiento de permanencia.

Fase 2: Modelado Predictivo (Machine Learning)
Preprocesamiento de datos

Para preparar los datos para los modelos predictivos se realizaron los siguientes pasos:

Eliminación de variables irrelevantes.

Conversión de variables categóricas a formato numérico.

Codificación de variables con One-Hot Encoding.

Mapeo de variables binarias.

División de datos

El dataset fue dividido en:

80% para entrenamiento

20% para prueba

Utilizando estratificación para preservar la proporción de la variable objetivo.

Escalado de variables

Las variables numéricas fueron normalizadas mediante StandardScaler para mejorar el rendimiento de los modelos.

Entrenamiento de modelos

Se entrenaron dos algoritmos de clasificación:

Regresión Logística

Random Forest

Evaluación de modelos

El rendimiento de los modelos fue evaluado utilizando:

Matriz de confusión

Precision

Recall

F1-score

AUC (Área bajo la curva ROC)

El modelo de Regresión Logística fue seleccionado como el modelo final debido a su mejor desempeño general.

Resultados del modelo

El modelo de Regresión Logística obtuvo los siguientes resultados:

AUC: 0.84

Recall: 0.52

Este resultado indica que el modelo tiene una buena capacidad para identificar clientes con riesgo de cancelación, lo cual es especialmente importante desde una perspectiva de negocio.

Variables más influyentes en la evasión de clientes

El análisis de importancia de variables, junto con la interpretación mediante SHAP, reveló los factores más determinantes en la cancelación del servicio.

Tipo de contrato

El contrato Month-to-month es el predictor más fuerte de abandono.

Antigüedad del cliente

Los clientes con menor tiempo en la empresa presentan mayor probabilidad de cancelar el servicio.

Tipo de servicio de internet

Los clientes con fibra óptica presentan una mayor tasa de cancelación.

Cargos del servicio

Los cargos mensuales elevados se relacionan con una mayor probabilidad de churn.

Soporte técnico

La ausencia de soporte técnico aumenta significativamente el riesgo de cancelación, especialmente en clientes con fibra óptica.

Plan de acción estratégico

A partir de los resultados obtenidos se proponen las siguientes acciones para reducir la tasa de cancelación.

Rediseñar la oferta de fibra óptica

Acción

Crear paquetes de fibra óptica que incluyan soporte técnico durante el primer año.

Objetivo

Mejorar la experiencia inicial del cliente y aumentar el valor percibido del servicio.

Incentivar contratos de largo plazo

Acción

Implementar campañas para incentivar a los clientes con contratos Month-to-month a migrar hacia planes anuales, ofreciendo beneficios como descuentos o meses gratuitos.

Objetivo

Reducir la probabilidad de cancelación y estabilizar la base de clientes.

Programa de acompañamiento para nuevos clientes

Acción

Implementar un programa de onboarding durante los primeros 90 días, especialmente para clientes de fibra óptica.

Objetivo

Fortalecer la relación con el cliente desde el inicio y mejorar su experiencia con el servicio.

Entregables del proyecto

El proyecto incluye:

Notebook de análisis exploratorio y modelado predictivo

Evaluación de modelos de Machine Learning

Interpretación de resultados con SHAP

Recomendaciones estratégicas basadas en datos

Conclusión

Este proyecto demuestra cómo un pipeline completo de ciencia de datos puede transformar datos empresariales en herramientas predictivas para la toma de decisiones.

La combinación de análisis exploratorio, modelado predictivo e interpretabilidad de modelos permite comprender no solo qué clientes abandonan la empresa, sino también por qué lo hacen y cómo prevenirlo.

De esta manera, el análisis de datos se convierte en un recurso clave para diseñar estrategias de retención más efectivas y basadas en evidencia.
