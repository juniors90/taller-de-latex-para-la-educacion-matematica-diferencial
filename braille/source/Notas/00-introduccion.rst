Introducción
===============

Los signos braille
----------------------------------

El lenguaje Braille se basa en una matriz de orden :math:`3\times 2`, tales que los :math:`6` puntos están numerados de la siguiente manera:

- Los puntos de la primer columna se numeran como :math:`1`, :math:`2` y :math:`3`, y

- Los de la segunda columna como :math:`4`, :math:`5` y :math:`6`, siempre de manera descendente (de arriba hacia abajo).

.. image:: img/matriz_braille.png
   :height: 578px
   :width: 432px
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

Por ejemplo, la letra "v minúscula" se forma en braille con los tres puntos :math:`(1236)`.

.. image:: img/alfabeto.png
   :height: 578px
   :width: 432px
   :scale: 30%
   :alt: matriz_braille
   :align: center



Notemos que, en la imagen anterior, los puntos :math:`4` y :math:`5` no forman parte de este signo, por lo que los señalamos con :math:`\textcolor{blue}{\blacksquare}`.


Pero ocurre que los signos visuales son muchos más que esas :math:`64` posibles combinaciones.

- :ref:`Alfabeto` (contempla las letras minúsculas y mayúsculas),
- :ref:`cifras-numericas`,
- :ref:`signos-de-puntuacion`,
- :doc:`04-operadores-aritmeticos` y
- :doc:`05-alfabeto-griego` (euro, porcentaje, etc.).


.. _Alfabeto-tex:

Archivo braille.sty
------------------------

Todas estas pruebas están desarrolladas bajo la programación del archivo ``braille.sty``, disponible para la descarga:

- :download:`docs/braille.sty`

En este archivo, por ejemplo, podemos encontrar la configuración de las letras griegas en el paquete ``braille``.

.. code-block:: latex
   
   % ---------------------------------------------------------------------------------------- %
   % Escritura de las letras del alfabeto Griego
   % ===========================================
   %
   % Minúsculas
   % ----------
   \prefix@char{4}{a}{alpha}      \prefix@char{4}{i}{iota}       \prefix@char{4}{r}{rho}
   \prefix@char{4}{b}{beta}       \prefix@char{4}{k}{kappa}      \prefix@char{4}{s}{sigma}
   \prefix@char{4}{g}{gamma}      \prefix@char{4}{l}{lambda}     \prefix@char{4}{t}{tau}
   \prefix@char{4}{d}{delta}      \prefix@char{4}{m}{mu}         \prefix@char{4}{u}{upsilon}
   \prefix@char{4}{e}{epsilon}    \prefix@char{4}{n}{nu}         \prefix@char{4}{f}{phi}
   \prefix@char{4}{z}{zeta}       \prefix@char{4}{x}{xi}         \prefix@char{4}{and}{chi}
   \prefix@char{4}{wh}{eta}       \prefix@char{4}{o}{omicron}    \prefix@char{4}{y}{psi}
   \prefix@char{4}{th}{theta}     \prefix@char{4}{p}{pi}         \prefix@char{4}{w}{omega}      
   % ---------------------------------------------------------------------------------------- %
   %
   % Mayúsculas
   % ----------
   \prefix@char{45}{a}{Alpha}      \prefix@char{45}{i}{Iota}       \prefix@char{45}{r}{Rho}
   \prefix@char{45}{b}{Beta}       \prefix@char{45}{k}{Kappa}      \prefix@char{45}{s}{Sigma}
   \prefix@char{45}{g}{Gamma}      \prefix@char{45}{l}{Lambda}     \prefix@char{45}{t}{Tau}
   \prefix@char{45}{d}{Delta}      \prefix@char{45}{m}{Mu}         \prefix@char{45}{u}{Upsilon}
   \prefix@char{45}{e}{Epsilon}    \prefix@char{45}{n}{Nu}         \prefix@char{45}{f}{Phi}
   \prefix@char{45}{z}{Zeta}       \prefix@char{45}{x}{Xi}         \prefix@char{45}{and}{Chi}
   \prefix@char{45}{wh}{Eta}       \prefix@char{45}{o}{Omicron}    \prefix@char{45}{y}{Psi}
   \prefix@char{45}{th}{Theta}     \prefix@char{45}{p}{Pi}         \prefix@char{45}{w}{Omega}


.. important::

   1. Una vez descargado este archivo, abrir con un editor de texto y copiar el contenido.

   2. Dirigirse a la ubicación del documento ``braile.sty``, dentro de la carpeta donde se ubica la distribución de latex, por ejemplo: 
   
      ``C:\Users\MY-USERNAME\AppData\Local\Programs\MiKTeX\tex\latex\braille\braille.sty``
   
   y pegar lo copieado en el paso anterior.

   3. Pegar el contenido a partir de la linea a partir de la linea ``155`` en adelante, para mantener el derecho de autor.


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