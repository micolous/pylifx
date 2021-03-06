******
pylifx
******

A Python library to control and monitor LIFX bulbs. Also provides a workaround
for users having issues with controlling LIFX bulbs on their network.

* GitHub: https://github.com/derkarnold/pylifx
* PyPi: https://pypi.python.org/pypi/pylifx

Originally written to allow the LIFX bulb to work in non-standard networks, but
it is growing to be much more.

Contributors: `Deryck Arnold <https://github.com/derkarnold>`_, `Michael Farrell (micolous) <https://github.com/micolous/>`_.

Huge thanks to `Kevin Bowman (magicmonkey) <https://github.com/magicmonkey/>`_ and others for the `lifxjs project on GitHub <https://github.com/magicmonkey/lifxjs/>`_.

Without their work on the lifxjs project, this one would not have been possible.

Current features
================

* Allows the LIFX bulb smartphone app to work by "faking" a bulb and relaying
  commands to the real one (see examples/bridge.py).

* Gives the ability to display the contents of LIFX messages coming through.

  * Huge thanks to magicmonkey and the lifxjs project for their hard work on
    working out the LIFX protocol.

* The ability to run "scenes" - provide a dictionary of times and colours and
  the library will do the rest (see examples/sunrise.py).

* Using multiple bulbs behind a single PAN gateway.

Upcoming features
=================

* Auto-discovery of bulbs (yes, should have been there already).

How to install
==============

* Get Python (tested with 2.7, others may work). I use the `Python(x, y) distribution <https://code.google.com/p/pythonxy/>`_.
* Ensure you have the Python setuptools.
* Run ``easy_install pylifx`` from a command prompt or terminal.
* You're done.

Two common issues with installing
---------------------------------

* **Linux users** - ensure you have python-dev installed (for the netifaces package).
* **Windows users** - install the pre-built binaries for your python distribution
  using the links in the following URL: http://alastairs-place.net/projects/netifaces/
  (The section is just above the start of the Changelog section).

Documentation
=============

If you don't want to build the documentation yourself, you can `view it online
<http://some-documentation-server.example.com/>`_.

Documentation may be built if you have `Sphinx <http://sphinx-doc.org/>`_.
You'll need to have pylifx built and in your ``PYTHON_PATH`` (or run Sphinx from
inside of a ``virtualenv`` that has it installed).  You can then build the HTML
documentation with:

.. code-block:: console

  $ cd doc
  $ make html

The documentation will then be available in ``doc/build/html/``.

There are other formats available, please see the Sphinx documentation for more
information.
