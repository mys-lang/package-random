|test|_

About
=====

Random numbers in the `Mys programming language`_.

Project: https://github.com/mys-lang/package-random

Examples
========

.. code-block:: python

   from random.pseudo import random
   from random.pseudo import randint
   from random.pseudo import randfloat
   from random.pseudo import randbytes

   def main():
       print("random():            ", random())
       print("randint(-5, 10):     ", randint(-5, 10))
       print("randfloat(-1.0, 3.5):", randfloat(-1.0, 3.5))
       print("randbytes(5):        ", randbytes(5))

API
===

Pseudo random numbers
---------------------

Cheap pseudo random numbers.

.. mysfile:: src/pseudo.mys

Cryptographically safe random numbers
-------------------------------------

Random numbers that should be cryptographically safe. Much slower than
pseudo random numbers.

.. mysfile:: src/crypto.mys

.. |test| image:: https://github.com/mys-lang/package-random/actions/workflows/pythonpackage.yml/badge.svg
.. _test: https://github.com/mys-lang/package-random/actions/workflows/pythonpackage.yml

.. _Mys programming language: https://mys-lang.org
