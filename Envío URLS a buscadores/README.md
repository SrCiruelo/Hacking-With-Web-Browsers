Existen vulnerabilidades que se pueden inyectar en la propia URL, SQL injection, XSS, Local File Include... .<br>
De forma que cualquier buscador puede indexar páginas con código malicioso como este, no solo es peligroso que aparezca
en los resultados de búsqueda si no que también el propio robot y su dominio se pueden ver afectados. <br>
***PD: Por esta última razón Google y Bing alojan la caché en un dominio alternativo y no el principal***

Además que el ataque sea realizado por un robot da más anonimato al atacante.

Si se usa un servicio como [Ping My URL](https://www.pingmyurls.com/) se añade aún más complejidad
para encontrar al atacante pues es un servicio automático sobre los robots de los buscadores.

### Redirecciones IP

Existen servicios como [bit.ly](https://bitly.com/) que permiten abreviar una url, de forma que los parámetros
de la petición que son maliciosos y fáciles de detectar, ya no son tan fáciles de ver a primera vista.

Además las redirecciones se pueden usar para aprovecharse del trabajo de otra gente.<br>
***Ej***
```
Si se devuelve una petición 301 Moved Permanently 
El robot imputará la página a la que se ha movido.

Sin embargo cuando se devuelve una petición 302 Moved Temporarily
El robot imputará la página movida temporalmente.
De esta forma el atacante puede referenciar páginas legítimas 
y útiles mejorando su posicionamiento.
```

Se puede redireccionar una página de forma que el robot entre en otra cuando pase por el dominio.
***Ej***
```
Definimos:
http://server0.com ==> url servidor normal 
http://server1.com/?user=%20getflag ==> url con vulnerabilidad de otro servidor

redirigimos server0 a esta url ==> http://server1.com/?user=%20getflag&d=

De esta forma cuando el robot intente acceder a http://server0.com/robots.txt realmente es
http://server1.com/?user=%20getflag&d=/robots.txt 

El parámetro d que tendría el valor /robots.txt se ignoraría.
De todas formas el buscador es probable que compruebe http://server1.com/robots.txt y que la 
URL http://server1.com/?user=%20getflag no se permita para que el robot no la indexe, de forma
que no tendríamos éxito.
```

EXALEAD es un buscador que ofrece thumbails antes de meterse en la página buscada y puede ayudar
para revisar una página sin ser descubierto.
