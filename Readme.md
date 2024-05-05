# Proyecto integrador 2

#### Introducción
En este trabajo integrador el objetivo es analizar las operaciones de un Call Center de un Banco, para proponer mejoras en:
* Eficiencia operativa, proponiendo mejoras operativas.
* Mejorar la satisfacción del cliente, cumpliendo los SLA comprometidos.
* Brindar una herramienta para la gestión y la toma de decisiones a los managers del Call Center.

  A la hora de analizar nos basaremos en las siguientes preguntas:
  
* ¿Cuál es el nivel de servicio para los clientes Prioritarios? 
* ¿Damos un mejor servicio que a los clientes normales? 
* ¿Qué volumen de llamadas atendemos? 
* ¿Cuáles son los cuellos de botella? ¿En qué días? ¿En qué bandas horarias? 
* ¿Cómo es la eficiencia y productividad de nuestros agentes? 
* ¿Hay clientes recurrentes en el uso del servicio? 
* ¿Cuáles son los tipos de servicio más recurrentes?
* ¿Podemos estimar la dotación necesaria para cumplir con una calidad de servicio determinada?  Ejemplo: si quiero que mi tiempo promedio de espera sea menor a 60 segundos?

  Este trabajo fue realizado integramente con Power Bi para poder aplicar todo lo aprendido en el M5.

## 1º Limpieza y validación de los datos
<div align="justify">
  En primer lugar se comienza con una limpieza de los datos para tener los mismos en la forma más conveniente para poder trabajar de manera eficaz y eficiente, además de descomponer algunas columnas codificadas y crear una tabla calendario.
  No se ahonda mucho en esta parte ya que la lista de  transformaciones está en Power Query dentro de Power BI.
</div>

  ## Conclusiones basadas en el Dashboard

  <div align="justify">
  En cuanto al trato respecto entre los clientes prioritarios y los de alta prioridad debemos comparar 3 etapas de la atención del callcenter.

  En primer lugar, en el tiempo medio que pasan en el VRU tanto entre ambos tipos de clientes no hay diferencias significativas.
  
  En el tiempo medio por que pasan los clientes en la fila de espera para ser atendidos lo clientes de alta prioridad tiene una media de 86,8 segundos mientras que los de prioridad regular tienen una media de 98,55 segundos lo que implica que los de lata prioridad tiene un timpo de cola de 11,9% menor que los de prioridad regular.
  
  En el tiempo del servicio por el agente los clientes de prioridad regular tienen un tiempo medio de 128,13 segundos mientras que los de alta prioridad 178,99 segundos. Entonces el el tiempo en servicio de los clientes de alta prioridad 39,7% mayor que los de prioridad regular.

  Entonces al analizar estos datos podemos ver como no hay una diferencia significativa en los timempos medios de VRU y en cola entre clientes regulares y de alta prioridad, e incluso en el tiempo medio de servicio es mas alto en los clientes de alta prioridad. Por lo que no se esta cunmpliendo con ell objetivo de darle un mejor servicio a un cliente con alta prioridad que paga un fee mensual.

  El volumen de llamadas recibidas en el año 1999 fue de 444448 donde aproximadamente el 47% de llamdas eran de clientes registrados. Los días con mayor volumen de llamadas se dan entre el Domingo y el Jueves y en esos días los horarios con mayor número de llamadas son de 6am a 7 pm. Mientras que los viernes el horario de mayor cantidad de llamadas es de 7 am a 3 pm. Los sabados los horarios con más volumen son de 7 pm a 12 am.

  Sobre los horarios antes mencionados el volumen es mucho más importante que en el resto de los horarios por lo que es importante tener en cuenta ya es princinpalmente en el primer periodo mencionado ya que es donde mayor porcentaje de clientes registrados llaman. Mientras que viernes y sabado el porcentaje de clientes que llaman es alrededor del 30%.

  En cuanto a los agentes, estos logran resolver el 78,3% de las consultas con un tiempo medio de servicio de 193,6 segundos o sea un poco mas de 3 minutos. También hay que destacar ciertos valores atípicos que habría que estudiar con mas atencion que suceden fuera del horario laboral donde están los agentes. Algo que es imposibles basicamente pero que habría que ahondar en el tema para ver si es un problema de toma de datos o algo más.

  En cuanto a los tipos de servicios, el más solicitado es la Actividad Regular con el 68%, luego le sigue los clientes potenciales solicitando mayor información con el 15,24% y último en el top 3 la actividad por acciones con el 8.85%. Si bien hay muchos clientes recurrentes también es importante notar la cantidad de clientes recurrentes que no llegan a completar el servicio. Esto es algo muy importante ya que el núumero es importante.
</div>

  ## Posibles mejoras

  <div align="justify">
    
1) - Lo pirmero que habría que mejorar o solucionar es el tema de la prioridad de los clientes. Tratar de llevar a cabo una campaña para registrar con exactitud las prioridades de los clientes para poder destinar recursos en primera medida a los clientes que abonan un fee con lo que se cumpliría con el servicio dado y mejoraría sustancialmente el tiempo de atención de los clientes de alta prioridad para asi lograr una diferencia mas evidente con los clientes regulares.

2) - Poder completar también aquellos ID de clientes que no están completos ya que muchos están en 0 y son probables clientes por lo que se vio no solo en las métricas sino también en el .txt que informaba sobre el problema.

3) - Sería muy importante tener información de los empleados y quien atiende cada llamada que llega a servicio para poder tener metricas de los desempeños individuales. Como también tener información mas detallada de los clientes.
    
4)  - Destinar más recursos a los horarios donde myor volumen de llamadas se detectan y revisar porque solo 2 VRU funcionaron ya que solo se tiene informacion de 2 de los 6 que había activos.

  </div>
  
  ## Conclusiones sobre el proyecto integrador

<div align="justify">
 Decidí hacer esta sección más allá de no ser requerida, ya que es mi primer experiencia en un proyecto de análisis de datos y creo que de alguna manera sirve para que al revisar lo que se ha hecho se han cometido errores y se han aprendido de los mismos.
  
 Es muy importante y creo que fundamental revisar los datos y diseñar por fuera de Power Bi una base de datos relacional, por ejemplo con Python. Ya que una vez que llegan los datos bien estructurados y bastante pulidos el análisis de simplifica muchísimo. Si bien uno puede ver en un principio de manera mas visual los datos dentro de la aplicacion de Microsoft creo que es mucho mas eficaz hacer un esquema por fuera del mismo.

 Si bien realice todo el trabajo sin utilizar Python, creo que para ahondar en muchas medidas es de vital importancia análisis estadísticos mas detallados y que pueden dar lugar a insights o findings mas profundos o específicos.
  </div>