Random
======

Random numbers in the `Mys programming language`_.

Examples
========

Cheap pseudo random numbers.

.. code-block:: python

   from random.pseudo import random
   from random.pseudo import randint
   from random.pseudo import randfloat
   from random.pseudo import randbytes

   def main():
       print('random():            ', random())
       print('randint(-5, 10):     ', randint(-5, 10))
       print('randfloat(-1.0, 3.5):', randfloat(-1.0, 3.5))
       print('randbytes(5):        ', randbytes(5))

.. code-block:: text

    random():             0.223932
    randint(-5, 10):      3
    randfloat(-1.0, 3.5): -0.31123
    randbytes(5):         b'\x34\xf4\x11\x92\xaa'

Random numbers that should be cryptographically safe. Much slower than
pseudo random numbers.

.. code-block:: python

   from random.crypto import random
   from random.crypto import randint
   from random.crypto import randfloat
   from random.crypto import randbytes

   def main():
       print('random():            ', random())
       print('randint(-5, 10):     ', randint(-5, 10))
       print('randfloat(-1.0, 3.5):', randfloat(-1.0, 3.5))
       print('randbytes(5):        ', randbytes(5))

.. code-block:: text

    random():             0.984442
    randint(-5, 10):      -5
    randfloat(-1.0, 3.5): 3.23477
    randbytes(5):         b'\x42\xff\x51\x89\xab'

.. _Mys programming language: https://github.com/mys-lang/mys
