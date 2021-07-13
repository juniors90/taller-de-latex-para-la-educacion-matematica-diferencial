Caracteres especiales
======================

Los caracteres especiales (acentos, tildes, etc.) conviene tener en cuenta que las letras que llevan diacríticos, tales como acentos y tildes, se escriben en Braille con una combinación de puntos distinta a la de la letra base del :doc:`01-alfabeto-braille`.

A continuación, se incluye una serie de comandos :math:`\LaTeX{}` donde aparecen las letras que llevan diacríticos en la escritura del idioma español (:ref:`vocales` y :ref:`letra-enie`)

.. _vocales:

Vocales con tilde
------------------

.. code-block:: latex
    
    % á
    \braille{{of}}      \\
    % é
    \braille{{the}}     \\
    % í
    \braille{{st}}      \\
    % ó
    \braille{{ing}}     \\
    % ú
    \braille{{with}}    \\

.. _letra-enie:

La letra ñ
------------

La letra ``ñ`` se escribe ``\braille{{er}}``

.. code-block:: latex
    
    \braille{{er}}

La letra ``Ñ`` se escribe ``\braille{{Italic}{er}}``

.. code-block:: latex
    
    \braille{{Italic}{er}}

La letra ü
------------

La letra ``ü`` se escribe ``\braille{{ou}}``

.. code-block:: latex
    
    \braille{{er}}


La letra ``Ü`` se escribe ``\braille{{Italic}{ou}}``

.. code-block:: latex
    
    \braille{{Italic}{ou}}