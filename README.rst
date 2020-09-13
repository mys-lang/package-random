|buildstatus|_

Random
======

Random numbers in the `Mys programming language`_.

Examples
========

.. code-block:: python

   from random import random
   from random import randint
   from random import randfloat

   def main():
       print('random():            ', random())
       print('randint(-5, 10):     ', randint(-5, 10))
       print('randfloat(-1.0, 3.5):', randfloat(-1.0, 3.5))

.. |buildstatus| image:: https://travis-ci.com/eerimoq/mys-random.svg?branch=master
.. _buildstatus: https://travis-ci.com/eerimoq/mys-random

.. _Mys programming language: https://github.com/eerimoq/mys
