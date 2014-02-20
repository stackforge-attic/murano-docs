Murano
======
Murano Project introduces an application catalog, which allows application
developers and cloud administrators to publish various cloud-ready
applications in a browsable‎ categorised catalog, which may be used by the
cloud users (including the inexperienced ones) to pick-up the needed
applications and services and composes the reliable environments out of them
in a “push-the-button” manner.

murano-docs
-----------
murano-docs repository contains different guides, manuals and documentation for
Murano project. Guides:

* Administrators Guide
* Developers Guide
* Getting Started Guide
* User Guide

Please, refer to `How to Build`_ sections for details about how to build guides
located in this repository.

Project Resources
-----------------
* `Murano at Launchpad <http://launchpad.net/murano>`__
* `Wiki <https://wiki.openstack.org/wiki/Murano>`__
* `Code Review <https://review.openstack.org/>`__
* `Sources <https://wiki.openstack.org/wiki/Murano/SourceCode>`__
* `Developers Guide <http://murano-docs.github.io/latest/developers-guide/content/ch02.html>`__

How To Participate
------------------
If you would like to ask some questions or make proposals, feel free to reach
us on #murano IRC channel at FreeNode. Typically somebody from our team will
be online at IRC from 6:00 to 20:00 UTC. You can also contact Murano community
directly by openstack-dev@lists.openstack.org adding [Murano] to a subject.

We’re holding public weekly meetings on Tuesdays at 17:00 UTC
on #openstack-meeting-alt IRC channel at FreeNode.

If you want to contribute either to docs or to code, simply send us change
request via `gerrit <https://review.openstack.org/>`__.
You can `file bugs <https://bugs.launchpad.net/murano/+filebug>`__ and
`register blueprints <https://blueprints.launchpad.net/murano/+addspec>`__ on
Launchpad.

How to Build
============
Prerequisites
-------------
`Apache Maven <http://maven.apache.org/>`_ must be installed to build the
documentation.

To install Maven 3 for Ubuntu 12.04 and later,and Debian wheezy and later::

    apt-get install maven

On Fedora 15 and later::

    yum install maven3


Build
-----
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

