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

#__PROBLEMAS DE SEGURIDAD__

Los problemas con la seguridad de la propia página puede ser un objetivo para los hackers que quieren 
mejorar el posicionamiento de sus páginas. 
