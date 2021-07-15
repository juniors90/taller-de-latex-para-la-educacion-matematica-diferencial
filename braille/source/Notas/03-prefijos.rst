Prefijos
==========

.. _minuscula:

Minúsculas
~~~~~~~~~~~

Con la fuente del Paquete Braille escribimos la palabra **jugar**:

.. code-block:: latex
    :caption: Ejemplo: escribimos la palabra jugar en Braille   
    
    \braille{jugar}

y esto nos devuelve los caracteres de las letras minúsculas descritas en el :doc:`01-alfabeto-braille`, formando la palabra jugar en Lenguaje Braille.

+---------------------------+---------------------------+---------------------------+---------------------------+---------------------------+
| j                         | u                         | g                         | a                         | r                         |
+---------------------------+---------------------------+---------------------------+---------------------------+---------------------------+
| .. figure:: img/pkg/j.svg | .. figure:: img/pkg/u.svg | .. figure:: img/pkg/g.svg | .. figure:: img/pkg/a.svg | .. figure:: img/pkg/r.svg |
|   :scale: 90%             |   :scale: 90%             |   :scale: 90%             |   :scale: 90%             |   :scale: 90%             |
|   :height: 100px          |   :height: 100px          |   :height: 100px          |   :height: 100px          |   :height: 100px          |
|   :width: 100%            |   :width: 100%            |   :width: 100%            |   :width: 100%            |   :width: 100%            |
|   :alt: braille           |   :alt: braille           |   :alt: braille           |   :alt: braille           |   :alt: braille           |
|   :align: left            |   :align: left            |   :align: left            |   :align: left            |   :align: left            |
+---------------------------+---------------------------+---------------------------+---------------------------+---------------------------+



.. _Mayuscula:

Mayúsculas
~~~~~~~~~~~~

Para las letras mayúsculas se utilizan las mismas signos que para las minúsculas, pero antes ha de escribirse el referido "prefijo de mayúscula" para indicar esta condición. La enumeración del prefijo de mayúscula en Braille está dada por :math:`(46)`.



+----------------------------------+-----------------------------------------+-----------------------------+
| En la Matriz                     | En el PDF                               | Comando  :math:`\LaTeX{}`   |
+==================================+=========================================+=============================+
| .. figure:: img/mayuscula.svg    | .. figure:: img/Braille6ANSI_may.svg    |  ``\braille{{Italic}}``     |
|   :scale: 40%                    |   :scale: 33%                           |                             |
|   :height: 100px                 |   :height: 100px                        |                             |
|   :width: 100%                   |   :width: 100%                          |                             |
|   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                             |
|   :align: center                 |   :align: center                        |                             |
|                                  |                                         |                             |
|   Puntos braille en la matriz    |   Signo Braille con Braille Package     |                             |
|                                  |                                         |                             |
+----------------------------------+-----------------------------------------+-----------------------------+

.. warning::

    Notar que para nuestro lenguaje castellano, entendemos por "Italic" al estilo *Itálica*. Es poco intuitivo scribir ``\braille{{Italic}}`` y que esto devuelva el prefijo de :ref:`Mayuscula`. Esto tiene que ver con varias causas

    1. El paquete Braille está pensado para usuarios que de habla Inglés.

    2. El lenguaje Braille puede cambia de un lenguaje hablado a otro.
    
    3. En el momento en que fue creado el paquete Braille tal vez no haya existido una conveción acerca del prefijo Mayúscula, entre otras.


