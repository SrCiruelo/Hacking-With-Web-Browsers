La campaña que sufrió la SGAE es un buen ejemplo de la importancia del SEO para una empresa.<br>
La campaña consistió en muchas personas refenciando en páginas a la SGAE con la url http://wwww.sgae.es/?ladrones (***la página es insegura por el uso de http, por cierto***), al refenciarse tanto el resultado fue que la página era la primera cuando se hacía la búsqueda ***"ladrones"***.<br>
Se intentó solucionar con un archivo robots.txt como este:

```
robots.txt
=====================
User-Agent: *
Allow:/

Disallow: /?
Disallow: /?ladrones
```
Este archivo, además de que es dudoso que funcione correctamente para todos los buscadores, solo es para los robots
de búsqueda y en el dominio propio, esto significa que los robots pueden conocer la url por otros medio, además 
de que por supuesto no evita que un usuario pueda acceder a la url aumentando la cantidad de personas que llegan a 
esa página a través de esa URL y así su relación con la palabra.

El problema se acabó solucionando entre la actuación directa de los empresas de buscadores y el olvido, o posiblemente 
cambio en los algoritmos de los buscadores.

Ser referenciado en páginas es algo buscado por los SEO y se puede hacer de forma fraudulenta 
__Spameando en foros,blogs,comentarios... etc.__ esto se puede remediar con etiquetas como: 
***\<meta name="robots" content="nofollow"\>***, que indican que los robots no deberían seguir 
ningún enlace referenciado dentro de la página o un atributo como: ***\<a href="google.com" rel="nofollow"\>***.<br>
De esta forma se deja inútil al spam.

### __PROBLEMAS DE SEGURIDAD__

Los problemas con la seguridad de la propia página puede ser un objetivo para los hackers que quieren 
mejorar el posicionamiento de sus páginas. 

Se pueden insertar elementos html en la propia página con referencias a las del páginas del hacker, por supuesto, 
el hacker no quiere que estos enlaces sean fácilmente visibles así que puede usar etiquetas como "style=display: none" 
estos elementos que no se ven en la página empeoran el ranking de nuestra página, cosa que el hacker tampoco quiere, pues 
le beneficiaría a él también, así que hacen usos de scripts para introducir elementos en la página de forma que no se pueda
empeorar el ranking en base al código introducido.

### __Cloaking forzado__

El Cloaking es una práctica que consiste en proporcionar distintos archivos html dependiendo de las cabeceras
de la petición del visitante, por ejemplo, dependiendo del user-agent dar una página u otra, de esta forma, cuando
un bot pase por la página leerá una página distinta que un usuario. 

Se puede hacer que dependiendo del referer se devuelva una página u otra, de forma que si se ha llegado por Google 
se devuelva una página normal y si se llega a través de una url devuelva una página de error. De forma que si se le envía 
un informe a un administrador de una página de una anomalía y se envía una url, este solo vería  un mensaje de error y pasaría 
a otro informe.

Esto se puede conseguir con el archivo ***.htcacces***

```.htcacces
RewriteEngine On 
RewriteCond %{HTPP_REFERER} google|bing
RewriteRule ^.*$http://xxxxxxxxxxxxxxxxxxx.com/item.php
```
También se pueden usar scripts, por ejemplo, php para conseguir más control al realizar Cloaking.

Para evitar esto, hay que revisar periodicamente el html de la página, además de realizar auditorías a 
la aplicación. 

Existen herramientas como ***"Bluefinder"*** que permite detectar de forma automática Cloaking.
