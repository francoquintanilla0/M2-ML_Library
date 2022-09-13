# M2-ML_Library

En este entregable se hace la implementación de una técnica de aprendizaje máquina (ML) con el uso de framework o biblioteca de aprendizaje máquina para la implementación de una solución. En este caso se optó por usar Random Forest Classifier en los datos del titanic.

Para este caso, después de hacer la limpieza de los datos NaNs y visualizar el comportamiento de los datos, implementamos el modelo de Random Forest, donde al estar experimentando con diferentes valores, el número de 20 árboles en nuestro bosque es el cual nos daba el mayor porcentaje de accuracy score.

Para poder hacer el análisis de nuestra técnica, dividimos nuestro dataset en 75% datos para entrenamiento y 25% datos para la evaluación, con un random state de: 1800 para poder obtener los mismos resultados en las diferentes corridas.

Consecuentemente, graficamos las variables a las cuales el modelo da mayor importancia, esto para observar el comportamiento que tiene con los distintos datos que le damos para entrenamiento y validación. Podemos observra que las caracteristicas más importantes son el sexo del pasajero, la cantidad de personas que lo acomañaban, y si era de primera o tercer clase en la que viajaba. 

Después de esto, hicimos algunas (5) predicciones para corroborar el Accuracy Score de nuestro modelo, las cuales nos dieron los siguientes resultados:

* Modelo 1
<img width="654" alt="Captura de Pantalla 2022-09-13 a la(s) 12 03 20" src="https://user-images.githubusercontent.com/111082680/189964006-20f00f3b-7147-4cbc-8f53-b49d15e56978.png">

* Modelo 2
<img width="640" alt="Captura de Pantalla 2022-09-13 a la(s) 12 03 25" src="https://user-images.githubusercontent.com/111082680/189964057-075c3aea-d69f-4099-875a-13f46334e45e.png">

* Modelo 3
<img width="637" alt="Captura de Pantalla 2022-09-13 a la(s) 12 03 30" src="https://user-images.githubusercontent.com/111082680/189964085-f7735c45-ad9d-433b-8160-9debafc20cd7.png">

* Modelo 4
<img width="637" alt="Captura de Pantalla 2022-09-13 a la(s) 12 03 36" src="https://user-images.githubusercontent.com/111082680/189964104-f1d6400b-7eac-4cad-b71a-ec9d72db04fc.png">

* Modelo 5
<img width="646" alt="Captura de Pantalla 2022-09-13 a la(s) 12 03 42" src="https://user-images.githubusercontent.com/111082680/189964142-8e80a6c2-d319-49d1-9778-a689a2be10b4.png">

En donde calculamos el Accuracy Score para cada uno, y los resultados fueron los siguientes:

<img width="285" alt="Captura de Pantalla 2022-09-13 a la(s) 12 03 49" src="https://user-images.githubusercontent.com/111082680/189964267-abb7b515-f669-428d-a581-0389c47bd3d0.png">

Después, calculamos la media de todos los Accuracy Scores, para ver que tan bien se desempeñaba el modelo, el resultado fue que la media de los Accuracy scores era del **0.8022**, lo cual es un resultado muy bueno.

Como podemos ver, el modelo que obtuvo un porcentaje de precisión más alto fue el de 82.58%, lo cual nos indica que es un modelo aceptable para la toma de decisiones en base al pensamiento estadístico. 

Después del análisis estadístico, una de las variables más importantes que nos regresa el modelo, es la importancia de cada una de sus variables, es decir, a cuales les da más peso/valor a ña hora de hacer el proceso de clasificación, en donde en nuestro caso del dataset, fueron las siguientes.

<img width="470" alt="Captura de Pantalla 2022-09-08 a la(s) 15 53 24" src="https://user-images.githubusercontent.com/111082680/189224181-921f74da-5253-4a0c-a88b-44ed24a7050a.png">

Como podemos ver, el sexo (masculino, femenino) es la variable con mayor peso en nuestro modelo.

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
