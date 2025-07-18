# T1-AI-Titanic
## Descripción
Este proyecto utiliza datos del famoso Titanic para practicar el análisis y manipulación de datos con Python, utilizando principalmente las librerías NumPy y Pandas en un entorno de Jupyter Notebook. El objetivo es explorar, limpiar y analizar los datos, así como realizar predicciones sobre la supervivencia de los pasajeros.

## Contenido del repositorio
- Notebook 1: Fundamentos de NumPy y Pandas
Ejercicios de manipulación de arrays con NumPy
Análisis de datos con Pandas usando datasets de ejemplo
Documentar cada celda con markdown explicativo

- Notebook 2: Visualizacion de datos
Visualización de los datos del Titanic usando distintas librerías gráficas.

- Notebook 3: Machine Learning:
Se aplican técnicas de machine learning para predecir la supervivencia de los pasajeros.

- Notebook 4: Dee_Learning
Se desarrollan y prueban modelos de deep learning para abordar el mismo problema.

## Resultados
### Notebook 1: Fundamentos de NumPy y Pandas 
Se listaron varios ejemplos de arrays y matrices en NumPy, mostrando su creación y algunos valores generados:
- Array desde una lista
- Un array de ceros, de tamaño 2x3
- Un array de unos, de tamaño 3x2
- Array usando linspace, 5 valores entre 0 y 10
- Arrays y matrices para operaciones

Con Pandas se obtuvieron datos para una estadistica descriptiva, para posteriormente realiar una agrupacion y calculos de medias.  Al agrupar los datos del Titanic por la columna Pclass (clase del pasajero), se obtienen las medias de Age (edad) y Fare (tarifa) para cada clase:
- Pclass	Edad media	Tarifa media
- 1	      38.23	        84.15
- 2	      29.88	        20.66
- 3	      25.14	        13.68
- Esto indica que los pasajeros de primera clase eran, en promedio, mayores y pagaban tarifas más altas que los de segunda y tercera clase (en donde se transportaba pasajeros de menos de 30 años y con menos recursos).

### Notebook 2: Visualizacion de datos
Se inicia con la verificación del entorno y versión de Python.
Se configura el estilo visual (paleta husl, fuentes, tamaños de gráfico).
Se instalan e importan las librerías necesarias, incluyendo herramientas para visualización avanzada y modelado básico.

Se usa sns.set(style="whitegrid") para mejor legibilidad.
Los gráficos ocultan bordes innecesarios (top y right) para estética minimalista.
Se establece un tamaño de gráfico estándar figsize=(10, 6) para uniformidad.

Existe fuerte sesgo de género y puerto de embarque.
La edad tiene distribución asimétrica, indicando alta presencia de adultos jóvenes.
Este tipo de análisis puede alimentar modelos predictivos posteriores (ej. predicción de supervivencia).

El notebook demuestra sólidamente las técnicas básicas de EDA y visualización para dos datasets clásicos.
Permite construir hipótesis preliminares para análisis posteriores o modelado.
La estructura es adecuada para enseñanza, prototipado y proyectos exploratorios en ciencia de datos.

### Notebook 3: Machine Learning:
. El modelo de machine learning entrenado en este notebook logra una precisión (accuracy) de 0.798 (aproximadamente 80%) en el conjunto de prueba.
Precisión global: 0.80
Promedio macro: 0.79
Promedio ponderado: 0.80
Estos resultados muestran un buen desempeño del modelo para predecir la supervivencia de los pasajeros del Titanic, con métricas balanceadas entre ambas clases.

. El modelo de regresión entrenado en este notebook obtuvo los siguientes resultados sobre el conjunto de evaluación:
Error cuadrático medio (MSE): 1742.76
Coeficiente de determinación (R²): 0.35
Estos valores indican que el modelo tiene una capacidad explicativa moderada sobre la variabilidad de los datos, aunque existe margen de mejora.

.  Se evaluaron varios algoritmos de machine learning para predecir la supervivencia en el Titanic. Los resultados de accuracy para cada modelo fueron:
Regresión Logística: 0.7978
Árbol de Decisión: 0.7416
Random Forest: 0.7640
SVM: 0.6854
El mejor desempeño se obtuvo con la Regresión Logística, alcanzando una precisión cercana al 80%.

### Notebook 4: Deep_Learning
El modelo de red neuronal fue entrenado con el dataset del Titanic durante 50 épocas, mostrando una mejora progresiva en la precisión desde 0.61 hasta alcanzar un valor máximo de 0.86 en el conjunto de entrenamiento. En cuanto a la validación, la precisión se estabilizó en torno a 0.80 a partir de la época 20, indicando un buen desempeño sostenido durante el entrenamiento.

Al evaluar el modelo con el conjunto de prueba, se obtuvo una precisión de 79.8% y una pérdida (loss) de 0.5111, lo que refleja que el modelo logra predecir correctamente la supervivencia de los pasajeros con un alto nivel de acierto.

En términos generales, los resultados sugieren que la red neuronal fue capaz de aprender patrones relevantes en los datos y generalizar de manera efectiva. La estabilidad en la precisión de validación y el buen resultado en test indican que el modelo no sufre de sobreajuste significativo.
## Autores
- José Raúl Avecillas Pacheco
- Juan Fernando Guzmán Quiñones
- Angélica Gabriela Prado Tixce
- Génesis Juliana Riera Naranjo
- Kevin Josué Villao Mendoza
