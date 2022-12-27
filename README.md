# PracticaCalificada4

## Pregunta 1

Se incorporará una nueva característica del producto en el entorno SOA que se muestra en la figura.

El CRM no tiene soporte para campañas de correo electrónico. Por lo tanto, se debe implementar un sistema para campañas de correo electrónico. Se sugiere que se creen dos servicios, uno para la creación y ejecución de campañas y un segundo servicio para evaluar los resultados de una campaña. Responde a las siguientes preguntas:

* ¿Se necesita la infraestructura SOA para integrar los dos nuevos servicios?

  Sí. Tanto la creación y ejecución de campañas como la evaluación de los resultados de estas son dos funcionalidades bien delimitadas que se deberían poder actualizar o reemplazar de forma independiente, por lo que conviene separarlas como servicios en esta arquitectura orientada a servicios.
  
* El servicio de evaluación de campañas necesita manejar una gran cantidad de datos. ¿Sería mejor utilizar la replicación de datos, la integración a nivel de interfaz de usuario o las llamadas de servicio para acceder a grandes cantidades de datos?
  
  La replicación de datos sería la peor opción, ya que son muchos y su replicación los haría inmanejables. La integración de estos servicios a nivel interfaz de usuario hace que no puedan operar de forma independiente, y esto es un problema al manejar grandes cantidades de datos. La mejor opción para el servicio de evaluación de campañas son las llamadas de servicio, pese a que esto ralentice un poco el proceso por los tiempos de espera en la comunicación.
   
* ¿Cuál de estas opciones de integración suele ofrecer SOA?
  
  La opción que más alineada está con los fundamentos de SOA la de las llamadas de servicio. Las otras opciones de integración mencionadas en la anterior pregunta también son ofrecidas por SOA.

* ¿Debe el servicio integrarse al portal existente o tener su propia interfaz de usuario?
 
  El servicio de evaluación de resultados de campañas deberia tener una propia interfaz de usuario para que así esta se pueda diseñar según los requerimientos particulares de su funcionalidad.

* ¿Cuáles son los argumentos a favor de cada opción?

  Para la segunda opción ya se comentó cuál es el argumento a favor. En cuanto a la opción de la integración al portal existente, el principal argumento a favor es que le facilita las cosas al usuario, ya que no tendrá que acceder a otro portal para usar el servicio y le resultará más familiar si se integra adecuadamente a dicho portal exixtente. En resumidas cuentas, tendría más usabilidad.

* ¿Debería implementar la nueva funcionalidad el equipo de CRM?

  Como se comentó en la primera pregunta, hay razones suficientes para implementar esta nueva funcionalidad como un servicio independiente. Ahora, ¿qué equipo debería implementarla? Obviamente el equipo de CRM debe estar involucrado en la implementación de este servivio de evaluación de campañas electrónicas, y si es un equipo de desarrolladores deben ser ellos quienes lo implementen.
  
## Pregunta 2

## Pregunta 3

## Pregunta 4

Ver el documento adjunto en este repositorio con el nombre «PC4 - Pregunta 4».
