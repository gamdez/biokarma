---
layout: post
title: Python. Función: isinstance()
---
isinstance(dato, tipo de datos)

interesante función que se sirve de 2 parámetros. El primero corresponde  a una variable que podría ser cualquier tipo de dato. El segundo parámetro es el grupo de datos con el cual queremos comprobar si el primer parámetro pertenece a éste tipo de grupo.

Entonces por ejemplo podríamos querer corroborar si un dato pertenece a los tipos de datos de Python como int, float, boolean, etc.

Ejemplo:
    
{% highlight ruby%}
>>> isinstance(1.0, float)
True
{% end highlight%}

