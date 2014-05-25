CMSPlugin for Django Outlets
============

Provides django-cms integration for django-outlets

Installation
------------

To get the latest stable release from PyPi

.. code-block:: bash

    pip install cmsplugin-django-outlets

To get the latest commit from GitHub

.. code-block:: bash

    pip install -e git+git://github.com/bitmazk/cmsplugin-django-outlets.git#egg=cmsplugin_outlets

TODO: Describe further installation steps (edit / remove the examples below):

Add ``cmsplugin_outlets`` to your ``INSTALLED_APPS``

.. code-block:: python

    INSTALLED_APPS = (
        ...,
        'cmsplugin_outlets',
    )

Add the ``cmsplugin_outlets`` URLs to your ``urls.py``

.. code-block:: python

    urlpatterns = patterns('',
        ...
        url(r'^outlets/', include('cmsplugin_outlets.urls')),
    )

Before your tags/filters are available in your templates, load them by using

.. code-block:: html

	{% load cmsplugin_outlets_tags %}


Don't forget to migrate your database

.. code-block:: bash

    ./manage.py migrate cmsplugin_outlets


Usage
-----

TODO: Describe usage or point to docs. Also describe available settings and
templatetags.


Contribute
----------

If you want to contribute to this project, please perform the following steps

.. code-block:: bash

    # Fork this repository
    # Clone your fork
    mkvirtualenv -p python2.7 cmsplugin-django-outlets
    make develop

    git co -b feature_branch master
    # Implement your feature and tests
    git add . && git commit
    git push -u origin feature_branch
    # Send us a pull request for your feature branch
