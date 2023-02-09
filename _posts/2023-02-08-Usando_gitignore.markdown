---
layout: post
title: Utilizando .gitignore
---

Sucede que haciendo un ejercicio quise crear un ambiente virtual tal y como era sugerido en éste; y como todo lo que hago lo 'subo' a github, me encontré con la pequeña sorpresa de que el montón de archivos creados para éste propósito (el ambiente virtual en éste caso crea una carpeta 'venv' con todas la configuraciones que necesita) también eran 'tomados' por git, para ser subidos como tal.

Ahora, esto me pasa porque por lo general para para añadir los archivos en los que he trabajado, lo hago todo de una vez de la siguiente manera:

{% highlight ruby %}
>>> git add -A
{% endhiglight%}

Añado para hacer ‘commit’ todos los archivos modificados hasta el momento. Una de las cosas que pude haber hecho para evitar que tomara la carpeta del ambiente virtual, pudo haber sido, indicar con git add solamente el archivo necesario.

{% highlight ruby %}
>>> git add archivo_para_hacer_commit
{% endhiglight%}

‘¿A qué me lleva toda esta explicación finalmente?’
 Simplemente que aprendí a que podemos ignorar lo que queramos que no sea tenido en cuenta con git. 

 ‘¿cómo se hace?’
 Creando un archivo llamado ‘.gitignore’, y dentro de éste, especificamos las terminaciones para los tipos de archivos, o las carpetas, etc que queremos no sean tenidos en cuenta.

'Un problema'
Tengo los proyectos en una carpeta, y a su vez, dentro de ésta carpeta los clasifico en otras. No sabía si podía crear un .gitignore que las cobijara a todas ubicándole en la 'carpeta madre' por llamarle así.  Cuando lo intenté hacer de esa manera, obtuve un error, y esto se debe al parecer a que en la carpeta madre no está instalado git.

Por lo pronto lo único que me funcionó fué crear el .gitignore dentro de la carpeta que utiliza proyectos o ejercicios con ambiente virtual.