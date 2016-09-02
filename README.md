# Puertos-distribuido

El proyecto socket funciona a partir de una dirección IP que ingrese el usuario y un rango de puertos, preguntará si estan disponibles esos puertos.
Para ayudar a esta tarea, el proyecto usa un mensaje broadcast para encontrar ayuda a partir del puerto 1234, si existe un servidor con este puerto que le conteste,
el proyecto toma la dirección IP del servidor y manda una petición TCP a la dirección que obtuvo con el puerto 5000, toma como garantizado que si le contestan el mensaje esa dirección tiene un servidor con el puerto 5000.


Nota: Para que funcione el proyecto no es necesario activar los servidores, pero si se desea realizar la tarea distribuida, es necesario activar ambos servidores en un equipo.
