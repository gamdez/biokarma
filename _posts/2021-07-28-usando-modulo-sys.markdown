---
layout: posts
title: Utilizando el módulo sys, para configurar una ruta (path)
categories: python
---

`El contexto:`
Escribiendo una GUI en particular, necesitaba utilizar código de un módulo
que se encuentra en otra carpeta. Es más fácil para mí trabajar de esta manera
pues el código del GUI puede llegar lo suficientemente denso, como para incluir
el mismo programa más líneas de código.

`La solución:`
Importar el módulo sys, y añadir una ruta hacia el código del módulo que queremos
utilizar en nuestro GUI de la siguiente manera.

{% highlight ruby %}
import sys
sys.path.append('/ruta/hacia/nuestro/modulo')
{% endhighlight %}
