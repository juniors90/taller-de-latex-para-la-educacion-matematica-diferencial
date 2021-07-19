Alfabeto Braille
==================



Alfabeto según el paquete Braille
----------------------------------

La siguiente es una lista de macros :math:`\TeX` y símbolos Braille contenidos en ``braille.sty``. El comando de usuario ``\braille{}`` convierte la secuencia de etiquetas en símbolos Braille.

- Una etiqueta puede ser un carácter que aparece tal cual, o varios caracteres que deben ir encerrados con ``{}``.

- Para cada etiqueta, se llama a una macro :math:`\TeX` predefinida para imprimir los símbolos Braille.

Por ejemplo,

.. code-block:: latex
    :caption: Macros
    
    \documentclass[draft, 12pt]{article}
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
| **a** | .. figure:: img/alph/letra_a.png | .. figure:: img/pkg/a.png               |  ``\braille{a}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **b** | .. figure:: img/alph/letra_b.png | .. figure:: img/pkg/b.png               |  ``\braille{b}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **c** | .. figure:: img/alph/letra_c.png | .. figure:: img/pkg/c.png               |  ``\braille{c}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **d** | .. figure:: img/alph/letra_d.png | .. figure:: img/pkg/d.png               |  ``\braille{d}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **e** | .. figure:: img/alph/letra_e.png | .. figure:: img/pkg/e.png               |  ``\braille{e}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **f** | .. figure:: img/alph/letra_f.png | .. figure:: img/pkg/f.png               |  ``\braille{f}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **g** | .. figure:: img/alph/letra_g.png | .. figure:: img/pkg/g.png               |  ``\braille{g}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **h** | .. figure:: img/alph/letra_h.png | .. figure:: img/pkg/h.png               |  ``\braille{h}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **i** | .. figure:: img/alph/letra_i.png | .. figure:: img/pkg/i.png               |  ``\braille{i}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **j** | .. figure:: img/alph/letra_j.png | .. figure:: img/pkg/j.png               |  ``\braille{j}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **k** | .. figure:: img/alph/letra_k.png | .. figure:: img/pkg/k.png               |  ``\braille{k}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **l** | .. figure:: img/alph/letra_l.png | .. figure:: img/pkg/l.png               |  ``\braille{l}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **m** | .. figure:: img/alph/letra_m.png | .. figure:: img/pkg/m.png               |  ``\braille{m}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **n** | .. figure:: img/alph/letra_n.png | .. figure:: img/pkg/n.png               |  ``\braille{n}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **o** | .. figure:: img/alph/letra_o.png | .. figure:: img/pkg/o.png               |  ``\braille{o}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **p** | .. figure:: img/alph/letra_p.png | .. figure:: img/pkg/p.png               |  ``\braille{p}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **q** | .. figure:: img/alph/letra_q.png | .. figure:: img/pkg/q.png               |  ``\braille{q}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **r** | .. figure:: img/alph/letra_r.png | .. figure:: img/pkg/r.png               |  ``\braille{r}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **s** | .. figure:: img/alph/letra_s.png | .. figure:: img/pkg/s.png               |  ``\braille{s}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **t** | .. figure:: img/alph/letra_t.png | .. figure:: img/pkg/t.png               |  ``\braille{t}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **u** | .. figure:: img/alph/letra_u.png | .. figure:: img/pkg/u.png               |  ``\braille{u}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **v** | .. figure:: img/alph/letra_v.png | .. figure:: img/pkg/v.png               |  ``\braille{v}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **w** | .. figure:: img/alph/letra_w.png | .. figure:: img/pkg/w.png               |  ``\braille{w}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **x** | .. figure:: img/alph/letra_x.png | .. figure:: img/pkg/x.png               |  ``\braille{x}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **y** | .. figure:: img/alph/letra_y.png | .. figure:: img/pkg/y.png               |  ``\braille{y}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **z** | .. figure:: img/alph/letra_z.png | .. figure:: img/pkg/z.png               |  ``\braille{z}``          |
|       |   :scale: 20%                    |   :scale: 20%                           |                           |
|       |   :height: 578px                 |   :height: 578px                        |                           |
|       |   :width: 432px                  |   :width: 432px                         |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+



.. _signos-de-puntuacion:

signos de puntuación
----------------------------------




.. _cifras-numericas:

Cifras Numéricas
----------------------------------
