---
layout: post
title: "Algo sobre diccionarios en Python"
categories: Python
---

# Usando la función dict()

![diccionario](/assets/leaf-icon.png)

Esto es una breve explicación sobre cómo en un caso específico, se dió uso a
esta función de una manera que me pareció muy interesante.

El ejemplo es utilizando el código Morse, el cuál una vez organizado en un
diccionario {letra: morse}, fué posible crear su equivalente {morse: letra}
usando esta función, lo que permite evitar tener que escribir un diccionario
completo nuévamente.

El diccionario para el código Morse sería el siguiente:

>abc_a_morse = {'a': '.-', 'b': '-...', 'c': '-.-.', 'd': '-..',
               'e': '.', 'f': '..-.', 'g': '--.', 'h': '....',
               'i': '..', 'j': '.---', 'k': '-.-', 'l': '.-..',
               'm': '--', 'n': '-.', 'o': '---', 'p': '.--.',
               'q': '--.-', 'r': '.-.', 's': '...', 't': '-',
               'u': '..-', 'v': '...-', 'w': '.--', 'x': '-..-', 'y',
                '-.--', 'z': '--..', '1': '.----', '2': '..---',
               '3': '...--', '4': '....-', '5': '.....', '6': '-....',
               '7': '--...', '8': '---..', '9': '----.', '0': '-----',
                ' ': ' ', '|': '|', "":""}

Ahora, para conseguir el diccionario con los valores de código Morse a letras,
bastaría con la siguiente línea de código:

> morse_a_abc = dict(value, key) for key, value in abc_a_morse.items())

y listo!

Fuente: Profesor Michael Eramo.
