# Análisis de Clientes (CHURN)
Este proyecto busca anticipar la probabilidad de que un cliente abandone una compañía, aplicando técnicas avanzadas de Machine Learning. Se realizó un análisis exploratorio de datos (EDA) y se implementaron diversos modelos para detectar patrones en el comportamiento de los clientes, proporcionando herramientas para mejorar las estrategias de retención.
## Tabla de Contenidos
- [Descripción del Proyecto](#descripción-del-proyecto)
- [Herramientas y Tecnologías](#herramientas-y-tecnologías)
- [Conjunto de Datos](#conjunto-de-datos)
- [Instrucciones de Instalación](#instrucciones-de-instalación)
- [Modelos Desarrollados](#modelos-desarrollados)
- [Resultados y Conclusiones](#resultados-y-conclusiones)
# Descripción del Proyecto
El análisis parte de un conjunto de datos obtenido de una hoja de cálculo en Google Sheets, el cual contiene información sobre el perfil y comportamiento de clientes. Se procesaron y limpiaron los datos, y se emplearon varios algoritmos de Machine Learning para predecir si un cliente continuará utilizando los servicios de la empresa o decidirá abandonarla.
# Herramientas y Tecnologías
Este proyecto emplea las siguientes herramientas y bibliotecas en Python:
* Python: Lenguaje principal para análisis y modelado.
* Pandas: Para el manejo y análisis de datos.
* NumPy: Soporte para operaciones numéricas y manipulación de arrays.
* Seaborn y Matplotlib: Creación de gráficos y visualizaciones.
* Scikit-learn: Implementación de algoritmos de Machine Learning.
* Keras: Construcción y entrenamiento de redes neuronales.
* XGBoost: Biblioteca especializada en modelos basados en árboles.
# Conjunto de Datos
La base de datos proviene de una hoja de Google Sheets identificada como Id_planilla = '1lJuHZIl-8iYOoi5cfYmnVoQq-RBl_2Yu2XIsqsjOvQA'. Contiene tanto datos demográficos como características del comportamiento de los clientes, además de una variable objetivo (Churn), que indica si un cliente ha abandonado la compañía (valor 1) o no (valor 0).
# Instrucciones de Instalación
Asegúrate de tener Python instalado en tu sistema. Para instalar las dependencias necesarias, ejecuta el siguiente comando en tu terminal:
bashpip install pandas numpy seaborn matplotlib scikit-learn keras xgboost
# Modelos Desarrollados
Se probaron diversos algoritmos para la predicción de churn, entre ellos:
1. Random Forest: Modelo basado en la combinación de múltiples árboles de decisión para mejorar la precisión.
2. Support Vector Machine (SVM): Clasificador que busca el mejor hiperplano para separar las clases.
3. Gradient Boosting: Modelo secuencial que optimiza errores de iteraciones previas.
4. XGBoost: Versión optimizada y eficiente de Gradient Boosting.
5. Redes Neuronales: Capaces de aprender patrones complejos a través de múltiples capas ocultas.
Cada modelo fue evaluado mediante métricas como matriz de confusión, F1-score y AUC-ROC.
# Resultados y Conclusiones
Entre los modelos evaluados, Gradient Boosting obtuvo el mejor desempeño con un AUC-ROC cercano a 0.8561, seguido por Random Forest, que logró un AUC-ROC de 0.8554. Estas métricas demuestran la capacidad de los modelos para identificar correctamente los clientes propensos a abandonar, proporcionando información valiosa para estrategias de retención.

