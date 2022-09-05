# M2-ML_Library

En este entregable se hace la implementación de una técnica de aprendizaje máquina (ML) con el uso de framework o biblioteca de aprendizaje máquina para la implementación de una solución. En este caso se optó por usar Random Forest Classifier en los datos del titanic.

Para este caso, después de hacer la liempieza de los datos NaNs y visualizar el comportamiento de los datos, implementamos el modelo de Random Forest, donde al estar experimentando con diferentes valores, el numero de 20 árboles en nuestro bosque es el cual nos daba el mayor porcentaje de accuracy score.

Para poder hacer el analisis de nuestra técnica, dividimos nuestro dataset en 75% datos para entrenamiento y 25% datos para la evaluación, con un random state de: 1800 para poder obtener los mismos resultados en las diferentes corridas.

Consecuentemente, graficamos las variables a las cuales el modelo da mayor importancia, esto para observar el comportamiento que tiene con los distintos datos que le damos para entrenamiento y validación. Podemos observra que las caracteristicas más importantes son el sexo del pasajero, la cantidad de personas que lo acomañaban, y si era de primera o tercer clase en la que viajaba. 

Por último, nuestro modelo obtuvo un porcentaje de precisión del 82.02%, lo cual nos indica que es un modelo aceptable para la toma de desiciones en base al pensamiento estadistico. 
