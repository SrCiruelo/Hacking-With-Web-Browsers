__Operadores de Búsqueda:__

+ "__str__". Busca exactamante str.
+ "__strA*strB__". Busca que exista strA y strB pero no necesariamente una seguida de otra.
+ "__strA__" AROUND(__N__) __strB__. Busca que exista strA y strB y que como mucho estén separadas por N palabras.
+ inurl: __str__. Busca una página con str en la url.
+ intitle: __str__. Busca una página con str en el título.
+ intext: __str__. Busca una página con str en el texto
+ site: __url__. Busca solo páginas del dominio indicado por url.
+ __strA__ OR __strB__. Funciona como el operador lógico OR.
+ __NUMA__..__NUMB__. Busca que numeros que estén en el rango [NUMA,NUMB]
+ filetype: __extension__. Busca archivos del tipo extension.
+ ext: __extension__. Busca archivos del tipo extension.
+ \- __operador: arg__. Hace el operador excluyente.
+ __filter=0__ en URL. Permite ver todos los resultados aunque sean muy parecidos 
+ link:"__domain__". Busca sitios referenciados por el dominio especificado.
[Más en operadores](https://support.google.com/websearch/?hl=es)

Si hacemos esta búsqueda=> inurl:security "phpmyadmin is free", podemos encontrar un sitio que nos cuenta
todo sobre la tecnología de sitio, además de cuentas de admin sin contraseña.

Webalizer: automatiza la tarea de crear estadísticas sobre el uso del sitio

Haciendo una búsqueda como esta '"usage statistics for" webalizer' podemos encontrar la información
del webalizer que nos muestras cosas como "/moodle/login/", dándonos a conocer que la página en cuestión,
usa moodle o incluso la ips para uso interno 193.201.227.20.

Haciendo la búsqueda "inurl:ws_ftp ext:ini intext:pwd", podemos encontrar páginas con el fichero WS_FTP.INI
que en sus versiones anteriores guardaba contraseñas encriptadas pero desencriptables.

Podemos excluir páginas que explican Google Hacking para una búsqueda usando por ejemplo, comandos 
como este: __-intitle:intitle__

Podemos usar la caché de Google para pasar desapercividos e incluso para ver información que ya no
está disponible, por otro lado tendremos es posible que tengamos información no actualizada.

Lo archivos con extensión .old son muy comunes para marcar un archivo como antiguo ,por ejemplo, index.old

A veces se deja a los bots acceder a páginas que normalmente una persona no tendría acceso, así que 
podemos cambiar nuestro user-agent para poder acceder aparentemente como un bot.

Se puede usar Google Docs para abrir de documentos de forma más segura.

Cuanto más se sepa, por ejemplo, de una tecnología mejores búsquedas podremos hacer Ejemplo:<br/>
   ***SMC-RZ30 HOME &nbsp;//Es una búsqueda que podemos usar para localizar webcams SONY***<br/>
   ***inurl:home/homeJ.html &nbsp;//Pero conociendo el sistema podemos hacer una mucha mejor búsqueda***<br/>


Podemos permanecer más despapercibidos si el campo Referer(***"Campo de la petición que indica de dónde proviene el visitante"***)
se mantiene, con la menor de cantidad de información posible,
***Ej, copiar una url de una búsqueda, abrir una nueva ventana y pegar la url ahí.***

Se puede usar Google para ver las páginas más actualizadas.

Existen los "Google Hacking Honeypots", páginas creadas para aparecer en los Google Dorks, que pueden ser utilizadas incluso
para cazar a posibles ciberdelincuentes.

Se pueden acceder a muchas cosas no solo relacionadas con el sitio que se va atacar en sí mismo, por ejemplo, manuales utilizados
para configurar los ordenadores de la empresa, facturas que indican el software del que hacen uso.

SiteDigger permite hacer búsquedas, además de contar con dos bases de datos de Google Dorks GHDB por un lado y la suya propia, hasta
facilita el uso de TOR para búsquedas.

Google Alerts permite "suscribirse" a búsquedas y avisará de cambios en los resultados de la búsqueda.

También se puede usar Google con un Feed RSS para realizar búsquedas automáticamente, suscriberse a cambios en webs y muchas más utilidades.

