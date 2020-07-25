__Operadores de Búsqueda:__

+ "__str__". Busca exactamante str.
+ "__strA__" near:__N__ "__strB__". Busca que exista strA y strB y que como mucho estén separadas por N palabras.
+ intitle: __str__. Busca una página con str en el título.
+ inbody: __str__. Busca una página con str en el texto
+ site: __url__. Busca solo páginas del dominio indicado por url y en directorios con un máximo de dos niveles de profundidad<br>
                ***Ej, Esta consulta no funcionará*** 
+ __strA__ OR __strB__. Funciona como el operador lógico OR.
+ __NUMA__..__NUMB__. Busca que numeros que estén en el rango [NUMA,NUMB]
+ filetype: __extension__. Busca archivos del tipo extension.
+ ext: __extension__. Busca archivos del tipo extension.
+ \- __operador: arg__. Hace el operador excluyente.
+ __filter=0__ en URL. Permite ver todos los resultados aunque sean muy parecidos 
[Más en operadores](https://docs.microsoft.com/en-us/previous-versions/bing/search/ff795634(v=msdn.10))
