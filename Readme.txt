
		==================================================================
   			  Actividad humana sobre el uso del Smartphone
		==================================================================


 El conjunto de datos incluye los siguientes ficheros:
 -----------------------------------------------------

- 'README.txt'

- 'features_info.txt': muestra informacion sobre las variables usadas.

- 'features.txt': Lista de todas las caracteristicas.

- 'activity_labels.txt': vector con el nombre de cada actividad.

- 'train/X_train.txt': conjunto de entrenamiento.

- 'train/y_train.txt': etiquetas del conjunto de entrenamiento

- 'test/X_test.txt': conjunto de prueba

- 'test/y_test.txt': etiquetas del conjunto de prueba


- 'train/subject_train.txt':  cada fila identifica al sujeto que realiza la actividad para cada muestra. Su rango es de 1 a 30.

- 'train/Inertial Signals/total_acc_x_train.txt': Señal de aceleración del eje X acelerómetro smartphones en 'g' unidades 						          de gravedad estándar. 
						  Cada fila muestra un elemento de un vector de tamaño 128. 
						  La misma descripción se aplica para el'total_acc_x_train.txt' y 								  'total_acc_z_train.txt'.

- 'train/Inertial Signals/body_acc_x_train.txt': La señal de aceleración del cuerpo obtenido restando la gravedad de la 						 aceleración total.

- 'train/Inertial Signals/body_gyro_x_train.txt': El vector de velocidad angular medida por el giroscopio para cada muestra                                                   Las unidades son radianes / segundo.




 
==============
    PASOS
==============


- Asignación del Directorio de trabajo

- Lectura de datos 'train' y datos 'test'

- Los datos "train" contienen la muestra de entrenamiento, que corresponde al 70% de la población, 
  formada por la unión de ficheros "train", mediante la función 'cbind' unimos las tablas por columnas

- Los datos "test" contienen la muestra de prueba, que corresponde al 30% de la población, 
  formada por la unión de ficheros "test" mediante la función 'cbind' unimos las tablas por columnas

- Formamos un único conjunto de datos, uniendo los datos de entrenamiento más los datos de prueba. 
  Esto lo haremos mediante la función 'rbind', lo que indica que la unión de ambas tablas se hará por filas, 
  ya que ambos conjuntos están formados por las mismas variables.

- Caluclo de la media y desviacion tipica para cada variable 

- Identificamos para el conjunto de datos, a que actividad corresponde cada observación

- Calculamos la Media por actividad e individuo
 
- Ordenamos el conjunto de datos en función del individuo y actividad
