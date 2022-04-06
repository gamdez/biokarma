---
layout: post
title: Usando enumerate en Python
---

Creando la nueva costumbre de escribir un poco acerca de la utilidad de
algunas funciones que me encuentro cuando lidio con mis pequeñeces (diarias?)
nos encontramos con algo interesante: **enumerate()**

Bueno, y para qué sirve? o mejor dicho, para qué lo he usado y cómo creo
que funciona? Realmente no soy la clase de persona que lee el manual completo, 
así que intentaré ser conciso.

Si tenemos una lista, por ejemplo 

{%highlight ruby%}
equipo = ['espada', 'brújula', 'lembas', 'escudo']
{%endhighlight%}

con enumeate podemos 'asignar' un número a cada cosa. Es como si tuviera
ahora un número de inventario asociado a cada elemento de nuestra lista,
en éste caso en particular el equipo.

si queremos 'imprimir' en pantalla haríamos lo siguiente:

{%highlight ruby%}
for numero, herramienta in enumerate(equipo):
	print('#: {}', herramienta: {}.format(numero, herramienta))
	
OUTPUT:
#: 0, herramienta: espada
#: 1, herramienta: brújula
#: 2, herramienta: lembas
#: 3, herramienta: escudo	
{%endhighlight%}

