__operadores de búsqueda:__
+ os: __nombre SO__. Busca equipos con el sistema operativo indicado.
+ port: __PORT NUMBER__. Busca equipos con el número de puerto indicado abierto.
+ country: __Country Code__.Busca equipos que estén el pais indicado.
+ city: __city name__.Busca equipos en la ciudad indicada.
+ after: __date__. Busca equipos de los que se tenga información a partir de la fecha dada. ***Ej,after: 22/03/2010***
+ before: __date__. Busca equipos de los que se tenga información antes de la fecha dada. ***Ej,before: 22/03/2010***
+ net: __ip/Mask__. Busca que la ip coincida con la dada. Mask funciona a modo de máscara de subred. **Ej,net:192.32.0.0/16<br> sólo buscara equipos cuya ip coincida con 192.32***
+ hostname: __nombre__. Busca equipos que en su nombre tenga el argumento dado.
+ html: __str__. Busca equipos que hostean web apps y busca que str se encuentre dentro de los archivos html.<br> Este operador tiene una capacidad de búsquedaa muy limitada.




***nmap*** es un programa que conociendo la ip de un servidor puede hacer un mapeo de la infraestructura de una red
y más datos que a los que pueda acceder.

Hay una cantidad preocupante de equipos con las credenciales por defecto.

En este buscador buscar un aparato sólo por el nombre de su modelo es bastante efectivo.

Las propias cabeceras de respuesta de un servidor puede darnos bastante información sobre este.

Se puede usar el número de puerto para hacerse una idea de la tecnología que se está usando, ya que aunque se pueden cambiar 
los puertos usados por una tecnología se suelen usar siempre los mismos.

Shodan tiene un buscador de exploits, e incluso informa de las posibles vulnerabilidades de los equipos buscados,
si conoce el software y la versión de este.
