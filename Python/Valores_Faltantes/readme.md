## Dataset utilizado
Se encuentra en Kaggle: [StudentAlcoholConsumption](https://www.kaggle.com/datasets/uciml/student-alcohol-consumption)  
Este dataset representa como el consumo de alcohol, entre otras variables, afectan el desempeño del estudiante en clases de matemáticas y portugués.  
El archivo se compone de 649 filas y 33 columnas que se componen de los siguientes elementos:  
•	school - escuela del estudiante (binario: 'GP' - Gabriel Pereira o 'MS' - Mousinho da Silveira)  
•	sex - sexo del estudiante (binario: 'F' - femenino o 'M' - masculino)  
•	age – edad del estudiante (numérico: del 15 al 22)  
•	address - tipo de domicilio del estudiante (binario: 'U' - urbano o 'R' - rural)  
•	famsize - tamaño de la familia (binario: 'LE3' – menor o igual a 3 o 'GT3' – mayor a 3)  
•	Pstatus - estado de convivencia de los padres (binario: 'T' - viven juntos o 'A' - separados)  
•	Medu - educación de la madre (0 - ninguna, 1 - educación primaria (4.º grado) 2 - 5.º a 9.º grado, 3 - secundaria 4 - educación superior)  
•	Fedu - educación del padre (0 - ninguna, 1 - educación primaria (4.º grado) 2 - 5.º a 9.º grado, 3 - secundaria 4 - educación superior)  
•	Mjob – trabajo de la madre ('teacher', 'health' care related, civil 'services' (ej. administrativo o policía), 'at_home' o 'other')  
•	Fjob – trabajo del padre ('teacher', 'health' care related, civil 'services' (ej. administrativo o policía), 'at_home' o 'other')  
•	reason – razon para escoger escuela (close to 'home', school 'reputation', 'course' preference o 'other')  
•	guardian - guardian del estudiante ('mother', 'father' o 'other')  
•	traveltime - tiempo de viaje de casa al centro ( 1 - 1 hora)  
•	studytime - tiempo de estudio semanal (1 - 10 horas)  
•	failures- número de clases  reprobadas en el pasado (numérico: n si 1<=n<3, o 4)  
•	schoolsup - apoyo educativo adicional (yes o no)  
•	famsup - apoyo educativo familiar (yes o no)  
•	paid - clases adicionales pagadas dentro de la asignatura (Matemáticas o Portugués) (binario: yes o no)  
•	activities - actividades extracurriculares (yes o no)  
•	nursery - asistió a la guardería (yes o no)  
•	higher - desea cursar estudios superiores (yes o no)  
•	internet - acceso a internet en casa (yes o no)  
•	romantic - tiene una relación romántica (yes o no)  
•	famrel - calidad de las relaciones familiares (de 1: muy mala a 5: excelente)  
•	freetime - tiempo libre después de la escuela (de 1: muy baja a 5: muy alta)  
•	goout - salir con amigos (de 1: muy baja a 5: muy alta)  
•	Dalc - consumo de alcohol en días laborales (de 1 - muy bajo a 5 - muy alto)  
•	Walc - consumo de alcohol en fin de semana (de 1 - muy bajo a 5 - muy alto)  
•	health - estado de salud actual (de 1 - muy malo a 5 - muy bueno)  
•	absences - número de ausencias escolares (de 0 a 93)   
#### Estas calificaciones están relacionadas con la asignatura, Matemáticas o Portugués:
• G1 - calificación del primer periodo (numérica: de 0 a 20)  
• G2 - calificación del segundo periodo (numérica: de 0 a 20)  
• G3 - calificación final (numérica: de 0 a 20, objetivo de resultados)  
________________________________________
## Descripción Proyecto
En este proyecto se realizan tres tratamientos de datos, un valor perdido, un outlier y diferentes análisis para llegar a una conclusión.  
Primero, un valor perdido, representa la ausencia de datos en una celda. Manejar correctamente estos valores incompletos es importante para la integridad y la validez de los resultados analíticos.   
Segundo, un Outlier (valor atípico) es una observación que se aleja considerablemente del resto de los datos. Puede representar errores o casos excepcionales.  
Finalmente se realizará un análisis exploratorio de datos, el cual usa métodos estadísticos para examinar un conjunto de datos; una correlación estadística que indica la relación entre variables y un modelo predictivo para llegar a una inferencia con respecto a la relación entre el consumo de alcohol y las calificaciones de estudiantes.
________________________________________
## Proyecto
Comienza importando diferentes librerías, numpy y pandas, para un mejor análisis, luego cargando el dataset a la plataforma.  
Sigue una identificación de valores faltantes, el cual, si bien no existen valores faltantes en este proyecto; si se utilizan diferentes métodos para encontrar valores perdidos, para demostrar conocimiento sobre la materia.  
Luego, se tratan los datos outliers, ya que, al eliminar los valores atípicos, la distribución es más limpia y simétrica, centrada en torno a 10–13. Esto facilita el análisis porque no se ven los valores poco representativos, que pueden distorsionar medidas estadísticas como la media o la desviación estándar.    
Por último, se realizan diferentes análisis para lograr inferir una relación entre las calificaciones de los alumnos y el consumo de alcohol.
________________________________________
## Conclusiones
  
•	Intercepto (const = 13.18)  
En promedio, un estudiante con consumo de alcohol diario y de fin de semana en el nivel más bajo (0) tendría una nota final de ~13,2.  

•	Dalc (coef = -0.54, p = 0.002)  
Cada incremento en el nivel de consumo diario de alcohol se asocia con una disminución de 0,54 puntos en G3, en promedio.  
Es estadísticamente significativo (p < 0.01).  
Esto indica que el consumo diario de alcohol tiene un efecto negativo en el rendimiento académico.  

•	Walc (coef = -0.20, p = 0.096)  
Cada incremento en el consumo de alcohol en fin de semana se asocia con una disminución de ~0,20 puntos en G3.  
Sin embargo, el efecto no es estadísticamente significativo al 5% (p ≈ 0.096).  
 Esto sugiere que el consumo en fines de semana podría afectar, pero la evidencia no es lo suficientemente fuerte.  

•	R² = 0.046 (4.6%)  
El modelo solo explica un 4,6% de la variabilidad de las notas finales.  
 Es decir, hay muchos otros factores (familiares, académicos, socioeconómicos, etc.) que influyen mucho más en G3.  

En conclusión, el consumo diario de alcohol (Dalc) sí tiene un efecto negativo significativo sobre el rendimiento académico. El consumo en fines de semana (Walc) muestra una tendencia negativa, pero no es concluyente estadísticamente. Aun así, el modelo explica poca varianza, por lo que el rendimiento escolar depende de más variables que solo el consumo de alcohol.

