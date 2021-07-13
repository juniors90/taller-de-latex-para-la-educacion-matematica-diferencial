Alfabeto Braille
==================

Los signos braille
----------------------------------

El lenguaje Braille se basa en una matriz de orden :math:`3\times 2`, tales que los :math:`6` puntos están numerados de la siguiente manera:

- Los puntos de la primer columna se numeran como :math:`1`, :math:`2` y :math:`3`, y

- Los de la segunda columna como :math:`4`, :math:`5` y :math:`6`, siempre de manera descendente (de arriba hacia abajo).

.. image:: img/matriz_braille.svg
   :height: 100px
   :width: 100%
   :scale: 30%
   :alt: matriz_braille
   :align: center

Un dato que me parece interesante es la mayoría de bibliografías señalan que, con una sola matriz, se pueden formar :math:`64` símbolos según estén presentes o no los puntos en cada matriz (incluyendo a la matriz vacía,que no tiene ningún punto). El hecho es que este número es el resultado del problema combinatorio subyacente que tiene como resultado:

.. math::

    \sum_{i=0}^{6} \left (\begin{array}{l} 6 \\ i \end{array}\right ) = 64

Entonces, ya sabemos que existen :math:`64` combinaciones posibles con una sola matriz, y cada una de estas son utilizadas para formar caracters simples con los cuales se pueden representar en Braille los signos gráficos que utilizamos para escribir textos impresos en caracteres visuales.


Enumeración de los puntos
~~~~~~~~~~~~~~~~~~~~~~~~~~~

La enumeración de los puntos que componen un signo Braille de un solo caracter se efectua mediante números de tantas cifras cuantos puntos sean utilizados, empleando para cada punto el dígito que lo identifica.

Por ejemplo, la letra "v minúscula" se forma en braille con los tres puntos :math:`(1,2,3,6)`.

.. image:: img/alfabeto.svg
   :height: 100px
   :width: 100%
   :scale: 30%
   :alt: matriz_braille
   :align: center



Notemos que, en la imagen anterior, los puntos :math:`4` y :math:`5` no forman parte de este signo, por lo que los señalamos con :math:`\textcolor{blue}{\blacksquare}`.


Pero ocurre que los signos visuales son muchos más que esas :math:`64` posibles combinaciones.

- :ref:`Alfabeto` (contempla las letras minúsculas y mayúsculas),
- :ref:`cifras-numericas`,
- :ref:`signos-de-puntuacion`,
- :doc:`03-operadores-aritmeticos` y
- :doc:`04-otros-signos-habituales` (euro, porcentaje, etc.).


.. _Alfabeto-tex:

Escritura en LaTeX
------------------------

Preámbulo
~~~~~~~~~~~~

.. code-block:: latex
    :caption: Preámbulo
    

    \documentclass[draft, 12pt]{article}
    %% ----------------------------  Inicio del Preámbulo  ---------------------------- %%
    \usepackage[spanish]{babel}
    \usepackage[utf8]{inputenc}
    \usepackage[T1]{fontenc}
    \usepackage{fullpage}
    \usepackage[puttinydots]{braille}
    
    \usepackage[lmargin=2.54cm, tmargin=2.54cm, rmargin=2.54cm, bmargin=2.54cm]{geometry}
    
    \title{Escritura con la Fuente Braille en \LaTeX{}}
    \author{Ferreira Juan David}
    \date{\today}
    %% ----------------------------  Fin del Preámbulo    ---------------------------- %%
    \begin{document}

    %%
    %% Cuerpo del documento.
    %%

    \end{document}

Alfabeto según el paquete Braille
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

La siguiente es una lista de macros :math:`\TeX` y símbolos Braille contenidos en ``braille.sty``. El comando de usuario ``\braille{}`` convierte la secuencia de etiquetas en símbolos Braille.

- Una etiqueta puede ser un carácter que aparece tal cual, o varios caracteres que deben ir encerrados con ``{}``.

- Para cada etiqueta, se llama a una macro :math:`\TeX` predefinida para imprimir los símbolos Braille.

Por ejemplo,

.. code-block:: latex
    :caption: Macros
    
    %% ----------------------------------------- %%
    %%        Aquí va nuestro Preámbulo          %%
    %% ----------------------------------------- %%

    \begin{document}

    \maketitle

    \section{Alfabeto Braille}
    % a 1
    \braille{a{the}b} \\

    \end{document}
    
imprime los símbolos Braille para ``a``, ``the`` y ``b``.

Como de costumbre, :math:`\TeX` colapsa varios espacios en un solo espacio e ignora los espacios al final de la línea y las pestañas y las nuevas líneas en todas partes. Esto significa que para el párrafo de varias líneas, debe haber al menos un espacio después de la nueva línea (``\n``).

.. _Alfabeto:

Escritura de las letras
------------------------

Escritura de los principales signos básicos con la fuente Braille Package.

+-------+----------------------------------+-----------------------------------------+---------------------------+
| Letra | Puntos braille en la matriz      | Signo según el Paquete Braille          | Comando                   |
+=======+==================================+=========================================+===========================+
| **a** | .. figure:: img/letra_a.svg      | .. figure:: img/pkg/a.svg               |  ``\braille{a}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **b** | .. figure:: img/letra_b.svg      | .. figure:: img/pkg/b.svg               |  ``\braille{b}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **c** | .. figure:: img/letra_c.svg      | .. figure:: img/pkg/c.svg               |  ``\braille{c}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **d** | .. figure:: img/letra_d.svg      | .. figure:: img/pkg/d.svg               |  ``\braille{d}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **e** | .. figure:: img/letra_e.svg      | .. figure:: img/pkg/e.svg               |  ``\braille{e}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **f** | .. figure:: img/letra_f.svg      | .. figure:: img/pkg/f.svg               |  ``\braille{f}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **g** | .. figure:: img/letra_g.svg      | .. figure:: img/pkg/g.svg               |  ``\braille{g}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **h** | .. figure:: img/letra_h.svg      | .. figure:: img/pkg/h.svg               |  ``\braille{h}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **i** | .. figure:: img/letra_i.svg      | .. figure:: img/pkg/i.svg               |  ``\braille{i}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **j** | .. figure:: img/letra_j.svg      | .. figure:: img/pkg/j.svg               |  ``\braille{j}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **k** | .. figure:: img/letra_k.svg      | .. figure:: img/pkg/k.svg               |  ``\braille{k}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **l** | .. figure:: img/letra_l.svg      | .. figure:: img/pkg/l.svg               |  ``\braille{l}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **m** | .. figure:: img/letra_m.svg      | .. figure:: img/pkg/m.svg               |  ``\braille{m}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **n** | .. figure:: img/letra_n.svg      | .. figure:: img/pkg/n.svg               |  ``\braille{n}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **o** | .. figure:: img/letra_o.svg      | .. figure:: img/pkg/o.svg               |  ``\braille{o}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **p** | .. figure:: img/letra_p.svg      | .. figure:: img/pkg/p.svg               |  ``\braille{p}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **q** | .. figure:: img/letra_q.svg      | .. figure:: img/pkg/q.svg               |  ``\braille{q}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **r** | .. figure:: img/letra_r.svg      | .. figure:: img/pkg/r.svg               |  ``\braille{r}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **s** | .. figure:: img/letra_s.svg      | .. figure:: img/pkg/s.svg               |  ``\braille{s}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **t** | .. figure:: img/letra_t.svg      | .. figure:: img/pkg/t.svg               |  ``\braille{t}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **u** | .. figure:: img/letra_u.svg      | .. figure:: img/pkg/u.svg               |  ``\braille{u}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **v** | .. figure:: img/letra_v.svg      | .. figure:: img/pkg/v.svg               |  ``\braille{v}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **w** | .. figure:: img/letra_w.svg      | .. figure:: img/pkg/w.svg               |  ``\braille{w}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **x** | .. figure:: img/letra_x.svg      | .. figure:: img/pkg/x.svg               |  ``\braille{x}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **y** | .. figure:: img/letra_y.svg      | .. figure:: img/pkg/y.svg               |  ``\braille{y}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **z** | .. figure:: img/letra_z.svg      | .. figure:: img/pkg/z.svg               |  ``\braille{z}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+


.. _prefijos:

Prefijos
-----------

.. _minuscula:

Minúsculas
~~~~~~~~~~~

Con la fuente del Paquete Braille escribimos la palabra **jugar**:

.. code-block:: latex
    :caption: Ejemplo: escribimos la palabra jugar en Braille   
    
    \braille{jugar}

y esto nos devuelve los caracteres de las letras minúsculas descritas en el Alfabeto_, formando la palabra jugar en Lenguaje Braille.

+---------------------------+---------------------------+---------------------------+---------------------------+---------------------------+
| j                         | u                         | g                         | a                         | r                         |
+---------------------------+---------------------------+---------------------------+---------------------------+---------------------------+
| .. figure:: img/pkg/j.svg | .. figure:: img/pkg/u.svg | .. figure:: img/pkg/g.svg | .. figure:: img/pkg/a.svg | .. figure:: img/pkg/r.svg |
|   :scale: 50%             |   :scale: 50%             |   :scale: 50%             |   :scale: 50%             |   :scale: 50%             |
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






.. _signos-de-puntuacion:

signos de puntuación
----------------------------------




.. _cifras-numericas:

Cifras Numéricas
----------------------------------
