X.509 Certificate to CybOX XML Converter
========================================

Generate CybOX XML from an X.509 Certificate file

**Version**: 0.2 BETA

    Copyright (c) 2013 - The MITRE Corporation
    All rights reserved. See LICENSE.txt for more details.

    BY USING THIS PROGRAM, YOU SIGNIFY YOUR ACCEPTANCE OF THE TERMS AND CONDITIONS
    OF USE.  IF YOU DO NOT AGREE TO THESE TERMS, DO NOT USE THIS PROGRAM.


Overview
--------

The X509-to-CybOX program parses an X.509 certificate (saved as plain text) and
creates a CybOX document containing a corresponding X509Certificate object.

Compatible with:
* [CybOX 2.0.1](http://cybox.mitre.org/language/version2.0.1/)

Installation
------------

Download and extract the included files into your directory of choice. 

X509-to-CybOX requires Python 2.X. It was developed using Python 2.7, and may work 
under Python 2.6. It is not compatible with Python 3.

### Dependencies 

* [python-cybox](https://pypi.python.org/pypi/cybox) - A Python library for CybOX

You can install the dependencies using pip:

    $ pip install cybox

**NOTE**: Installing LXML (which python-cybox depends on) on Ubuntu requrires the
python-dev, libxml2-dev, and libxslt1-dev packages to be installed. 
Follow the link for instructions on installing python-cybox and LXML on Windows.

Usage
-----

    python x509_to_cybox.py -i <x509 cert txt file> -o <cybox xml file>

### Example files

X509-to-CybOX comes with example input and output files. You can use these to see an example
of the program's output, or to verify that you have installed to program correctly:

    $ python x509_to_cybox.py -i examples/x509.in.txt -o x509.xml
    $ diff x509.xml examples/x509.out.xml

More information
----------------

* CybOX - http://cybox.mitre.org/
