===============
 stevedore 0.3
===============

.. tags:: stevedore release python

What is stevedore?
==================

Python makes loading code dynamically easy, allowing you to configure
and extend your application by discovering and loading extensions
("*plugins*") at runtime. Many applications implement their own
library for doing this, using ``__import__`` or
``importlib``. stevedore_ avoids creating yet another extension
mechanism by building on top of `setuptools entry points`_. The code
for managing entry points tends to be repetitive, though, so stevedore
provides manager classes for implementing common patterns for using
dynamically loaded extensions.

.. _stevedore: http://stevedore.readthedocs.org

.. _setuptools entry points: http://packages.python.org/distribute/pkg_resources.html#convenience-api


What's New?
===========

- Added dispatch managers for selecting among a set of plugins at
  runtime instead of load time.
- Added ``__call__`` method to ``DriverManager`` so it can be invoked
  in a more natural fashion for a single plugin.

Installing
==========

Visit the stevedore_ project page for download links and installation
instructions.
