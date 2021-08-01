|discord|_
|test|_
|stars|_

About
=====

Random numbers in the `Mys programming language`_.

Project: https://github.com/mys-lang/package-random

Examples
========

Use pseudo random numbers.

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

Build and run:

.. code-block:: myscon

   ❯ mys run
    ✔ Reading package configuration (0 seconds)
    ✔ Building (0.01 seconds)
   random():             0.898648
   randint(-5, 10):      1
   randfloat(-1.0, 3.5): 2.61118
   randbytes(5):         b"\x40\x27\x00\x2e\x47"

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

.. |discord| image:: https://img.shields.io/discord/777073391320170507?label=Discord&logo=discord&logoColor=white
.. _discord: https://discord.gg/GFDN7JvWKS

.. |test| image:: https://github.com/mys-lang/package-random/actions/workflows/pythonpackage.yml/badge.svg
.. _test: https://github.com/mys-lang/package-random/actions/workflows/pythonpackage.yml

.. |stars| image:: https://img.shields.io/github/stars/mys-lang/package-random?style=social
.. _stars: https://github.com/mys-lang/package-random

.. _Mys programming language: https://mys-lang.org
