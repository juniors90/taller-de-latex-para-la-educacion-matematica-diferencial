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
| **a** | .. figure:: img/alph/letra_a.svg | .. figure:: img/pkg/a.svg               |  ``\braille{a}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **b** | .. figure:: img/alph/letra_b.svg | .. figure:: img/pkg/b.svg               |  ``\braille{b}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **c** | .. figure:: img/alph/letra_c.svg | .. figure:: img/pkg/c.svg               |  ``\braille{c}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **d** | .. figure:: img/alph/letra_d.svg | .. figure:: img/pkg/d.svg               |  ``\braille{d}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **e** | .. figure:: img/alph/letra_e.svg | .. figure:: img/pkg/e.svg               |  ``\braille{e}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **f** | .. figure:: img/alph/letra_f.svg | .. figure:: img/pkg/f.svg               |  ``\braille{f}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **g** | .. figure:: img/alph/letra_g.svg | .. figure:: img/pkg/g.svg               |  ``\braille{g}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **h** | .. figure:: img/alph/letra_h.svg | .. figure:: img/pkg/h.svg               |  ``\braille{h}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **i** | .. figure:: img/alph/letra_i.svg | .. figure:: img/pkg/i.svg               |  ``\braille{i}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **j** | .. figure:: img/alph/letra_j.svg | .. figure:: img/pkg/j.svg               |  ``\braille{j}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **k** | .. figure:: img/alph/letra_k.svg | .. figure:: img/pkg/k.svg               |  ``\braille{k}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **l** | .. figure:: img/alph/letra_l.svg | .. figure:: img/pkg/l.svg               |  ``\braille{l}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **m** | .. figure:: img/alph/letra_m.svg | .. figure:: img/pkg/m.svg               |  ``\braille{m}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **n** | .. figure:: img/alph/letra_n.svg | .. figure:: img/pkg/n.svg               |  ``\braille{n}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **o** | .. figure:: img/alph/letra_o.svg | .. figure:: img/pkg/o.svg               |  ``\braille{o}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **p** | .. figure:: img/alph/letra_p.svg | .. figure:: img/pkg/p.svg               |  ``\braille{p}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **q** | .. figure:: img/alph/letra_q.svg | .. figure:: img/pkg/q.svg               |  ``\braille{q}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **r** | .. figure:: img/alph/letra_r.svg | .. figure:: img/pkg/r.svg               |  ``\braille{r}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **s** | .. figure:: img/alph/letra_s.svg | .. figure:: img/pkg/s.svg               |  ``\braille{s}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **t** | .. figure:: img/alph/letra_t.svg | .. figure:: img/pkg/t.svg               |  ``\braille{t}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **u** | .. figure:: img/alph/letra_u.svg | .. figure:: img/pkg/u.svg               |  ``\braille{u}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **v** | .. figure:: img/alph/letra_v.svg | .. figure:: img/pkg/v.svg               |  ``\braille{v}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **w** | .. figure:: img/alph/letra_w.svg | .. figure:: img/pkg/w.svg               |  ``\braille{w}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **x** | .. figure:: img/alph/letra_x.svg | .. figure:: img/pkg/x.svg               |  ``\braille{x}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **y** | .. figure:: img/alph/letra_y.svg | .. figure:: img/pkg/y.svg               |  ``\braille{y}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **z** | .. figure:: img/alph/letra_z.svg | .. figure:: img/pkg/z.svg               |  ``\braille{z}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+








.. _signos-de-puntuacion:

signos de puntuación
----------------------------------




.. _cifras-numericas:

Cifras Numéricas
----------------------------------
