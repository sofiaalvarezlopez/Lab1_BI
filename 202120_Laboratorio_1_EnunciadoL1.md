# Laboratorio 1 - Clasificación

## Objetivos

 - Comprender el proceso asociado a la preparación de datos para una tarea de clasificación. 
 - Utilizar una herramienta para el preprocesamiento, la limpieza, el perfilamiento de los datos y la construcción, evaluación, interpretación y uso del modelo.
 - Analizar e identificar los hiperparámetros adecuados para los modelos de clasificación propuestos.
 - Comparar 3 clasificadores utilizados y seleccionar uno que justifican y recomiendan a la organización.
 - Obtener conclusiones a nivel técnico y organizacional, a partir de los modelos generados.
 - Comunicar los hallazgos encontrados a la organización y explicar por qué tienen valor para el negocio.
 
## Herramientas
Durante este laboratorio trabajaremos con las siguientes herramientas:


 - Python
	 - Distribución sugerida: [Anaconda](https://www.continuum.io/downloads) 
		 - La versión de Anaconda es 4.4
		 - La versión usada es la de python 2.7, usar la de python 3 no debería requerir muchos cambios. 
	 - Ambiente de desarrollo
	   	 - JupyterLab
	 - Librerías
	 	 - Pandas
		 - Scikit-learn
		 - Matplot
		 - Seaborn

## Enunciado 
SaludAlpes es una entidad de salud colombiana que se especializa en atender pacientes diagnosticados con diabetes. 
Entre las actividades principales de SaludAlpes se destaca el análisis de resultados de laboratorio para la detección de diabetes. 
Este servicio de diagnóstico implica el análisis manual por parte de médicos especialistas, a partir de los resultados de exámenes de laboratorio, lo cual ha generado en los últimos años, una serie de problemas asociados con los tiempos de atención a estos pacientes, causada por demoras en la confirmación del diagnóstico. 
SaludAlpes los ha contratado para agilizar y mejorar el proceso de análisis de resultados clínicos de tal manera que se reduzcan los tiempos de confirmación de diagnóstico y se agilice el inicio del tratamiento a paciente con diabetes confirmada. 
Su labor como consultor de BI es agilizar el proceso de confirmación de diagnóstico de diabetes en un paciente, utilizando datos históricos y realizando sobre ellos procesos de análisis y procesamiento, al igual que comunicando los resultados a la entidad para afianzar sus conocimientos en áreas de aprendizaje automático y al mismo tiempo generar una ventaja competitiva.

Con el fin de lograr el objetivo para el cual fue contratado, SaludAlpes espera tener tres modelos distintos de clasificación, construidos con 3 técnicas diferentes, entre las cuales deben estar árboles de decisión y KNN (k-nearest-neighbours). De igual manera, espera que siga la metodología que ellos utilizan en la actualidad para el desarrollo de ese tipo de proyectos, 
para lo cual le sugiere realizar los siguientes pasos:

1.	Descargar y entender los datos [SaludAlpes_diagnosticos_dataset.csv](datos/SaludAlpes_diagnosticos_dataset.csv) utilizando el [diccionario de datos](datos/SaludAlpes_diagnosticos_dataset_dictionary.pdf).
2.	Realizar un análisis exploratorio y perfilamiento de datos que le permita entenderlos, al igual que identificar el nivel de calidad de los datos y las tareas de transformación que se requieren para construir modelos de clasificación utilizando técnicas como KNN y árboles de decisión entre otras. 
Adicionalmente, la entidad desea incluir como entregable, tableros de control para apoyar tareas de entendimiento de datos y nivel de calidad de los mismos, para lo cual sugiere mostrar estadisticas tales como cantidad de columnas, cantidad de datos, valores nulos, promedio de cada variable entre otros posibles datos que puedan proveer información útil a SaludAlpes.
3.	Describir y justificar el preprocesamiento que debe realizar para limpiar los datos y dejarlos listos para aplicar los algoritmos asociados con el uso de 3 técnicas de clasificación.
4.	Construir tres clasificadores diferentes con el uso de: K nearest-neighbours, árboles de decisión y uno de libre elección que permita clasificar los conjuntos de datos de manera correcta. 
En este punto, deben justificar las decisiones más importantes asociadas al proceso, tales como los criterios utilizados para la selección de hiperparámetros y las modificaciones a los datos para construir cada clasificador.
5.	Analizar los resultados obtenidos y justificar la utilidad de estos modelos para SaludAlpes.
6.  Comparar los distintos modelos obtenidos y explicar cuál recomendarían a SaludAlpes.
7.	Desarrollar una presentación donde expongan sus resultados y recomendaciones a SaludAlpes.


### Ejemplo de posible tablero de control
![img](img/Dashboard-ej.JPG)

## Entregables 

 - Documento con todos los puntos que debe realizar en el laboratorio. 
 Incluya adicionalmente, el nombre del estudiante que realizó cada uno de los clasificadores. Por ejemplo, Felipe Gonzalez realizó el modelo basado en KNN. De igual manera, cada estudiante, debe incluir una descripción general de la forma como funciona el clasificador utilizado.
 - Presentación con los resultados obtenidos (punto 7).
 - Notebook que contiene el proceso realizado.
 - Archivo que contiene el tablero de control creado.

## Instrucciones de Entrega

Recuerde hacer la entrega por la sección unificada en Bloque Neón, antes del sábado 4 de septiembre a las 22:00.   
Este será el único medio por el cual se recibirán entregas.

## Rúbrica de Calificación

A continuación se encuentra la rúbrica de calificación.

**Nota:** Los siguientes porcentajes hacen referencia a la nota grupal, que corresponde a un 80% de la nota inidiviudal.  
El 20% restante se calcula según el puntaje obtenido en la implmenetación del algoritmo del cual el estudiante estuvo a cargo dentro del grupo.

| Concepto | Porcentaje |
|:---:|:---:|
| Descripción y análisis del perfilamiento de los datos y de las tareas sugeridas de transformación | 20% |
| Descripción del preprocesamiento realizado, según el algoritmo utilizado | 10% |
| Implementación de Arboles de decision, descripción de las decisiones más importantes asociadas a la implementación del algoritmo y los hiperparametros configurados | 7% |
| Implementación de K-NN, descripción de las decisiones más importantes asociadas a la implementación del algoritmo y los hiperparametros configurados | 7% |
| Implementación de un tercer algoritmo de libre elección, descripción de las decisiones más importantes asociadas a la implementación del algoritmo y los hiperparametros configurados | 12% |
| Análisis de los resultados obtenidos y justificación del modelo recomendado para el caso propuesto | 30% |
| Presentación para SaludAlpes con resultados y recomendaciones dadas a la empresa | 10% |
| Notebook asociado | 5% |
  


## Documentación de scikit-learn de apoyo
- [scit-learn](https://scikit-learn.org/stable/supervised_learning.html#supervised-learning)

## Sugerencias

 - Nota 1: Como lo habrá notado, en los datos entregados hay atributos categóricos. Para poder realizar el proceso de clasificación hay que tratar estos valores.
 - Nota 2: Revisar el diccionario de datos y entender los valores posibles de las columnas en este tipo de examenes clínicos.
 - Nota 3: Analizar si los valores de cada columna corresponden a valores adecuados para el negocio, en caso de que no lo sean, deben tratar dichos valores y justificar sus decisiones.
 - Nota 4: Utilizar los datos que sean útiles para determinar un posible diagnóstico de diabetes.
 - Nota 5: Para el preprocesamiento de los datos y los tableros de control se puede hacer uso de las herramientas del curso o de otras herramientas diferentes según el criterio propio.
 

## ACLARACIONES
 - Cada integrante del grupo debe estar encargado de la implementación de un clasificador distinto. Sin embargo, todos los integrantes del grupo deben tener la capacidad de explicar lo realizado por los demás compañeros y determinar la mejor solución para SaludAlpes. 
 - El análisis de resultados y su justificación debe ser realizado en grupo.
 - Las notas de los integrantes dentro de un mismo grupo de laboratorio pueden variar ya que en los puntos 3 y 4 cada integrante está encargado de la implementación de un clasificador distinto. 
 


 


