pefile-to-maec
==============

A Python library for converting output from Ero Carrera's `pefile <https://code.google.com/p/pefile/>`_ utility to MAEC XML content.  It is currently in the pre-release phase.

:Source: https://raw.githubusercontent.com/MAECProject/pefile-to-maec/master/pefile_to_maec.py
:MAEC: http://maec.mitre.org
:CybOX: http://cybox.mitre.org

Dependencies
------------

**python-maec** |maec version badge| |maec downloads badge|

**python-cybox** |cybox version badge| |cybox downloads badge|

.. |maec version badge| image:: https://pypip.in/v/maec/badge.png
   :target: https://pypi.python.org/pypi/maec/
.. |maec downloads badge| image:: https://pypip.in/d/maec/badge.png
   :target: https://pypi.python.org/pypi/maec/
.. |cybox version badge| image:: https://pypip.in/v/cybox/badge.png
   :target: https://pypi.python.org/pypi/cybox/
.. |cybox downloads badge| image:: https://pypip.in/d/cybox/badge.png
   :target: https://pypi.python.org/pypi/cybox/

Overview
--------

pefile-to-maec employs the `python-maec <https://pypi.python.org/pypi/maec/>`_ and `python-cybox <https://pypi.python.org/pypi/cybox/>`_ for the conversion to MAEC.

"pefile is a multi-platform Python module to read and work with Portable Executable (aka PE) files. Most of the information in the PE Header is accessible, as well as all the sections, section's information and data."[1]

Compatibility
-------------

The pefile-to-maec library is tested and written against python ``2.7.x``. Compatibility with other python versions is neither guaranteed nor implied.

Installation
------------

The pefile package does not require any external libraries if run from the 
command line.
If installing from source, ``setuptools`` is required.  You can also install pefile from within the Ubuntu package repository:

-  python-pefile

The ``maec`` package depends on the following Python libraries: \* ``lxml`` >=
3.1.x \* ``python-cybox`` >= 2.1.x.x \* ``setuptools`` (only if installing
using setup.py)

For Windows installers of the above libraries, we recommend looking here:
http://www.lfd.uci.edu/~gohlke/pythonlibs. python-cybox can be found at
https://github.com/CybOXProject/python-cybox/releases.

To build ``lxml`` on Ubuntu, you will need the following packages from the
Ubuntu package repository:

-  python-dev
-  libxml2-dev
-  libxslt1-dev

For more information about installing lxml, see
http://lxml.de/installation.html

Features
--------

- metadata
    - file name (on disk)
    - file path
    - file size (in bytes)
    - hashes (md5, sha1)
- dos header
- file header
- optional header
- exports
- imports
- resource directories

References
----------

[1]: https://code.google.com/p/pefile/

Feedback
--------

Bug reports and feature requests are welcome and encouraged. Pull requests are
especially appreciated. Feel free to use the issue tracker on GitHub or send an
email directly to maec@mitre.org.
