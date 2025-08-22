##Dataset utilizado

Se encuentra en Kaggle: [StressLevelDataset](https://www.kaggle.com/datasets/mdsultanulislamovi/student-stress-monitoring-datasets)

Este dataset representa el estres en estudiantes midiendo diferentes variables como: Niveles de ansiedad, autoestima, etc.
El archivo se compone de 1100 filas y 21 columnas que se componen de:
anxiety_level, self_esteem, mental_health_history, depression, headache, 
blood_pressure, sleep_quality, breathing_problem, noise_level, living_conditions, safety, basic_needs, academic_performance, study_load, teacher_student_relationship,
future_career_concerns, social_support, peer_pressure, extracurricular_activities, bullying, stress_level

__________________________________________________________________________________________________________________
##Decripción Proyecto

Este proyecto presenta un análisis IDA, EDA, estadística descriptiva para el análisis de datos, análisis de correlación de datos y creación de gráficos.
Estos análisis tienen como objetivo resolver las siguientes preguntas:

Análisis de datos
• ¿Qué factores se reportan más seguido?
• ¿Cuántos estudiantes han reportado antecedentes de problemas de salud mental?
• ¿Cuál es el nivel promedio de ansiedad de los estudiantes en el conjunto de datos?
• ¿Cuáles son los 3 mayores factores que aumentan al estrés?
• ¿Para el factor que disminuye el estres, cuántos estudiantes tienen un nivel por debajo del promedio?
• ¿Cuáles son los 3 factores que disminunyen el estrés?

Análisis comparativo
• ¿Cuáles con las correlaciones entre los factores?
• ¿Los estudiantes que sufren acoso escolar tienen mayor probabilidad de tener antecedentes de problemas de salud mental?

_____________________________________________________________________________________________________________________
##Proyecto 

Comienza importando diferentes librerias para un mejor análisis, luego cargando el dataset a la plataforma. Sigue un analisis IDA, este conjunto de datos no contiene valores faltantes ni duplicados.
No requiere limpieza, por lo que se puede comenzar el análisis sin pasos adicionales.
Continua con estadistica descriptiva, creación de gráficos para un análisis de datos más claros y
por ultimo, se termina con un análisis comparativo. Gracias a todo lo anterior se puede llegar a una conclusión de los factores y
experiencias de los estudiantes que afectan el estres.
_____________________________________________________________________________________________________________________
##Desarrollo

Análisis de datos
• ¿Qué factores se reportan más seguido?
Los factores más reportados son los académicos, que incluyen: 'academic_performance', 'study_load', 'teacher_student_relationship', 'future_career_concerns'.

• ¿Cuántos estudiantes han reportado antecedentes de problemas de salud mental?
542 alumnos presentan historial de problemas de salud mental, lo que representa un 49.32%.

• ¿Cuál es el nivel promedio de ansiedad de los estudiantes en el conjunto de datos?
El nivel de ansiedad promedio tiene una puntuacion 11, de una escala del 0 al 21.

• ¿Cuáles son los 3 mayores variables que aumentan al estrés?
Las 3 variables que aumentan el nivel de estres son: 1) Bullying 2) Nivel de ansiedad 3)Preocupaciones futuras de carrera.

• ¿Cuáles son los 3 mayores variables que disminunyen el estrés?
Las variables que disminuyen el nivel de estres son: 1) Autoestima 2) Calidad de sueño 3) Rendimiento académico

• ¿Para la variable que más disminuye el estres, cuántos estudiantes tienen un nivel por debajo del promedio?
El número de estudiantes que estan bajo el promedio es 507, con un porcentke de 46.13%

Análisis comparativo
• ¿Cuáles con las correlaciones entre las variables?
Dirigirse al mapa de calor dentro del proyecto, para una visión clara de las correlaciones.

_______________________________________________________________________________________________________________________
##Conclusiones
