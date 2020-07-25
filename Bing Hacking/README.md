__Operadores de Búsqueda:__

+ "__str__". Busca exactamante str.
+ "__strA__" near:__N__ "__strB__". Busca que exista strA y strB y que como mucho estén separadas por N palabras.
+ intitle: __str__. Busca una página con str en el título.
+ inbody: __str__. Busca una página con str en el texto
+ site: __url__. Busca solo páginas del dominio indicado por url y en directorios con un máximo de dos niveles de profundidad<br>
                ***Ej, Si queremos encontrar "health.news.my_page.com" Esta consulta no funcionará "site:my_page.com" *** 
+ site: __url__. Busca solo páginas del dominio indicado por url.<br>
                ***Ej, Si queremos encontrar "health.news.my_page.com" Esta consulta si funcionará "domain:my_page.com" *** 
+ __strA__ OR __strB__. Funciona como el operador lógico OR.
+ filetype: __extension__. Busca archivos del tipo extension y no tiene en cuenta su extensión.
+ ext: __extension__. Busca archivos con la extensión indicada.
+ contains: __extension__. Busca documentos que tienen enlaces a ficheros de la extensión dada.
+ \- __operador: arg__. Hace el operador excluyente.
+ instreamset(__url|body|title|anchor__):__str__ .Busca que los resultados contengan str en el sition indicado. 
[Más en operadores](https://docs.microsoft.com/en-us/previous-versions/bing/search/ff795634(v=msdn.10))

La búsqueda avanzada en Bing es muy parecida a la de Google.

Con el operador ***"contains:"*** podemos encontrar páginas no indexadas por robots.***'contains:log ws_ftp intitle:"index of"'***

