=============================
django-webex
=============================

.. image:: https://badge.fury.io/py/django-webex.svg
    :target: https://badge.fury.io/py/django-webex

.. image:: https://travis-ci.org/yourname/django-webex.svg?branch=master
    :target: https://travis-ci.org/yourname/django-webex

.. image:: https://codecov.io/gh/yourname/django-webex/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/yourname/django-webex

An open-source Cisco Webex (teams) plugin for Django.

Documentation
-------------

The full documentation is at https://django-webex.readthedocs.io.

Quickstart
----------

Install django-webex::

    pip install django-webex

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'django_webex.apps.DjangoWebexConfig',
        ...
    )

Add django-webex's URL patterns:

.. code-block:: python

    from django_webex import urls as django_webex_urls


    urlpatterns = [
        ...
        url(r'^', include(django_webex_urls)),
        ...
    ]

Features
--------

* TODO

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox


Development commands
---------------------

::

    pip install -r requirements_dev.txt
    invoke -l


Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
