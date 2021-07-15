Caracteres especiales
======================

Los caracteres especiales (acentos, tildes, etc.) conviene tener en cuenta que las letras que llevan diacríticos, tales como acentos y tildes, se escriben en Braille con una combinación de puntos distinta a la de la letra base del :doc:`01-alfabeto-braille`.

A continuación, se incluye una serie de comandos :math:`\LaTeX{}` donde aparecen las letras que llevan diacríticos en la escritura del idioma español (:ref:`vocales` y :ref:`letra-enie`)

.. _vocales:

Vocales con tilde
------------------

+-------+----------------------------------+-----------------------------------------+---------------------------+
| Letra | Puntos braille en la matriz      | Signo según el Paquete Braille          | Comando                   |
+=======+==================================+=========================================+===========================+
| **á** | .. figure:: img/dia/ad.svg       | .. figure:: img/dia/ad_pkg.svg          |  ``\braille{a}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **é** | .. figure:: img/dia/ed.svg       | .. figure:: img/dia/ed_pkg.svg          |  ``\braille{a}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **í** | .. figure:: img/dia/id.svg       | .. figure:: img/dia/id_pkg.svg          |  ``\braille{a}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **ó** | .. figure:: img/dia/od.svg       | .. figure:: img/dia/od_pkg.svg          |  ``\braille{a}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+
| **ú** | .. figure:: img/dia/ud.svg       | .. figure:: img/dia/ud_pkg.svg          |  ``\braille{a}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+





.. _letra-enie:

La letra ñ
------------

+-------+----------------------------------+-----------------------------------------+---------------------------+
| Letra | Puntos braille en la matriz      | Signo según el Paquete Braille          | Comando                   |
+=======+==================================+=========================================+===========================+
| **ñ** | .. figure:: img/dia/enie.svg     | .. figure:: img/dia/enie_pkg.svg        |  ``\braille{a}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+

La letra ``ñ`` se escribe ``\braille{{er}}``

.. code-block:: latex
    
    \braille{{er}}

La letra ``Ñ`` se escribe ``\braille{{Italic}{er}}``

.. code-block:: latex
    
    \braille{{Italic}{er}}

.. _letra-uu:

La letra ü
------------

+-------+----------------------------------+-----------------------------------------+---------------------------+
| Letra | Puntos braille en la matriz      | Signo según el Paquete Braille          | Comando                   |
+=======+==================================+=========================================+===========================+
| **ü** | .. figure:: img/dia/uu.svg       | .. figure:: img/dia/uu_pkg.svg          |  ``\braille{a}``          |
|       |   :scale: 40%                    |   :scale: 33%                           |                           |
|       |   :height: 100px                 |   :height: 100px                        |                           |
|       |   :width: 100%                   |   :width: 100%                          |                           |
|       |   :alt: puntos_matriz_braille    |   :alt: matriz_braille                  |                           |
|       |   :align: center                 |   :align: center                        |                           |
+-------+----------------------------------+-----------------------------------------+---------------------------+

La letra ``ü`` se escribe ``\braille{{ou}}``

.. code-block:: latex
    
    \braille{{er}}


La letra ``Ü`` se escribe ``\braille{{Italic}{ou}}``

.. code-block:: latex
    
    \braille{{Italic}{ou}}