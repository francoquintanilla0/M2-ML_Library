# M2-ML_Library

En este entregable se hace la implementación de una técnica de aprendizaje máquina (ML) con el uso de framework o biblioteca de aprendizaje máquina para la implementación de una solución. En este caso se optó por usar Random Forest Classifier en los datos del titanic.

Para este caso, después de hacer la limpieza de los datos NaNs y visualizar el comportamiento de los datos, implementamos el modelo de Random Forest, donde al estar experimentando con diferentes valores, el número de 20 árboles en nuestro bosque es el cual nos daba el mayor porcentaje de accuracy score.

Para poder hacer el análisis de nuestra técnica, dividimos nuestro dataset en 75% datos para entrenamiento y 25% datos para la evaluación, con un random state de: 1800 para poder obtener los mismos resultados en las diferentes corridas.

Consecuentemente, graficamos las variables a las cuales el modelo da mayor importancia, esto para observar el comportamiento que tiene con los distintos datos que le damos para entrenamiento y validación. Podemos observra que las caracteristicas más importantes son el sexo del pasajero, la cantidad de personas que lo acomañaban, y si era de primera o tercer clase en la que viajaba. 

Por último, nuestro modelo obtuvo un porcentaje de precisión del 82.02%, lo cual nos indica que es un modelo aceptable para la toma de decisiones en base al pensamiento estadístico. 

Para saber el comportamiento de nuestro modelo modelo, utilizamos las siguientes aplicaciones:

* Learning Curve
* Confusion Matrix

En donde los resultados fueron los siguientes:

**Learning Curve**

<img width="382" alt="Captura de Pantalla 2022-09-08 a la(s) 15 42 00" src="https://user-images.githubusercontent.com/111082680/189222421-b621c0fd-a54e-4510-82a2-be0007b1ad89.png">

En donde podemos ver como nuestro modelo empieza un poco abajo, pero va aprendiendo hasta llegar a su punto más óptimo de aprendizaje sin llegar a un overfitting, pero tampoco tan simple como para quedarse estancado en el underfitting.

**Confusion Matrix**

<img width="349" alt="Captura de Pantalla 2022-09-08 a la(s) 15 47 37" src="https://user-images.githubusercontent.com/111082680/189222883-feaf4e75-1820-4832-8f1f-e34f10065250.png">

En donde podemos observar la cantidad de verdaderos positivos, verdaderos negativos, falsos negativos, falsos positivos. Que en este caso nuestro modelo hace un buen trabajo en determinar predicciones.
