### Robtex

Robtex es una apliccación web que permite conseguir información sobre dominios, ips relacionadas con los dominios.

Haciendo uso de Robtex podemos encontrar las ips que pertenecen a un relacionadas con un dominion.<br>
***Ej, Encontramos que las ips 150.203 son ips pertenecientes a anu.edu de forma que podemos hacer***
***una búsqueda en Google del tipo 150.203.\*.\* para encontrar más información sobre la organización objetivo, o incluso***
***hacer uso del operador ip de bing***

### Descifrar Contraseñas

En internet hay una cantidad inmensa del hash contraseñas comunes y hay algunos hash como md5 o SHA1.<br>
***Ej, Encontramos la contraseña hasheada 5f4dcc3b5aa765d61d8327deb882cf99 en una página web, con hacer una búsqueda rápida***
***nos encontramos con que 5f4dcc3b5aa765d61d8327deb882cf99 es el hash para password.***

De hecho hay buscadores específicos para la búsqueda de hashes la herramienta gratuita más versátil: [CrackStation](https://crackstation.net/).

### Reconocer ataques ya realizados

Podemos usar las herramientas de webmaster de bing [Bing Webmasters](https://www.bing.com/toolbox/webmaster) 
para explorar los enlaces creados por ciberdelincuentes.<br>
Existen más herramientas aunque su funcionalidad sin pagar es reducida.[ahrefs](https://ahrefs.com/es/)[LinkPad](https://linkpad.org/default.aspx)

### Pasar desapercibido sin caché

Podemos usar un buscador como [waybackmachine](https://archive.org/web/) para acceder al contenido de la
página sin ser detectados, cuando esto no es posible podemos hacer uso del índice ("descripción rápida del buscador")

***Ej***
```
Search: 0xword
==============================
Nos da este índice
==============================

"Inicio. Lista de las paginas en Inicio: Política de Privacidad · Entrega · Aviso legal · Condiciones de uso · 0xWORD · Pago seguro · Publica tu libro"

==============================
Podemos usar las últimas palabras para ver el siguiente índice 
==============================

Search: site:https://0xword.com/es/3_0xword "Publica tu libro"
==============================
Nos da este nuevo índice
==============================

Política de Privacidad · Entrega · Aviso legal · Condiciones de uso · 0xWORD · Publica tu libro · Distribuidores y Librerias · [Manual de instalación]. Controle su ...

==============================
Así podríamos leer toda la página pero puede ser que unas palabras coincidan y nos devuelvan un índice
ya leído.
==============================

Search: site:https://0xword.com/es/3_0xword "Controle su *"
==============================
* nos puede sacar de este aprieto, incluso usando varios seguidos.
AROUND también nos puede ayudar
==============================

==============================
Si finalmente no conseguimos más resultados podemos cambiar de navegador.
==============================

==============================
Si cambiar de navegador no funciona, ya solo queda hacer búsquedas con palabras que es muy probable que aparezcan
==============================
```
