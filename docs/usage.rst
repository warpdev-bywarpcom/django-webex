=====
Usage
=====

To use django-webex in a project, add it to your `INSTALLED_APPS`:

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
