Murano Manuals
+++++++++++++++++

This repository contains documentation for the
Murano project. It includes:

 * API Specification
 * Architecture
 * Installation

For more details, see the `Murano <http://murano-docs.github.io>`_.


Prerequisites
=============
`Apache Maven <http://maven.apache.org/>`_ must be installed to build the
documentation.

To install Maven 3 for Ubuntu 12.04 and later,and Debian wheezy and later::

    apt-get install maven

On Fedora 15 and later::

    yum install maven3


Building
========
The different manuals are in subdirectories of the
``docs/src/`` directory.

To build a specific guide, look for a ``pom.xml`` file within a subdirectory,
then run the ``mvn`` command in that directory. For example::

    cd docs/src/developers-guide
    mvn clean generate-sources

The generated PDF documentation file is::

    docs/src/developers-guide/src/target/docbkx/pdf/developers-guide.pdf

The root of the generated HTML documentation is::

    docs/src/developers-guide/src/target/docbkx/webhelp/developers-guide/content/index.html


Installing
==========
Refer to http://murano.openstack.org Learn more about the Murano project.
