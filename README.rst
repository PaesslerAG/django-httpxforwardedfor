=============================
django-httpxforwardedfor
=============================

.. image:: https://travis-ci.org/PaesslerAG/django-httpxforwardedfor.svg?branch=master
        :target: https://travis-ci.org/PaesslerAG/django-httpxforwardedfor

----

.. contents:: Set request.META['REMOTE_ADDR'] from request.META['HTTP_X_FORWARDED_FOR']

----

Quickstart
----------

Install django-httpxforwardedfor::

    pip install django-httpxforwardedfor

Then use it in a project::

    import httpxforwardedfor

Release Notes
-------------

* 0.1.0 - initial release (2017-04-12)

  * supports Django 1.8, 1.9, 1.10, 1.11 on python 2.7, 3.3, 3.4, 3.5, and 3.6 - as per the
    `official django docs <https://docs.djangoproject.com/en/dev/faq/install/#what-python-version-can-i-use-with-django>`_


.. contributing start

Contributing
------------

As an open source project, we welcome contributions.

The code lives on `github <https://github.com/PaesslerAG/django-httpxforwardedfor>`_.

Reporting issues/improvements
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Please open an `issue on github <https://github.com/PaesslerAG/django-httpxforwardedfor/issues/>`_
or provide a `pull request <https://github.com/PaesslerAG/django-httpxforwardedfor/pulls/>`_
whether for code or for the documentation.

For non-trivial changes, we kindly ask you to open an issue, as it might be rejected.
However, if the diff of a pull request better illustrates the point, feel free to make
it a pull request anyway.

Pull Requests
~~~~~~~~~~~~~

* for code changes

  * it must have tests covering the change. You might be asked to cover missing scenarios
  * the latest ``flake8`` will be run and shouldn't produce any warning
  * if the change is significant enough, documentation has to be provided

Setting up all Python versions
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

::

    sudo apt-get -y install software-properties-common
    sudo add-apt-repository ppa:fkrull/deadsnakes
    sudo apt-get update
    for version in 3.3 3.5 3.6; do
      py=python$version
      sudo apt-get -y install ${py} ${py}-dev
    done

Code of Conduct
~~~~~~~~~~~~~~~

As it is a Django extension, it follows
`Django's own Code of Conduct <https://www.djangoproject.com/conduct/>`_.
As there is no mailing list yet, please just email one of the main authors
(see ``setup.py`` file or `github contributors`_)


.. contributing end


.. _github contributors: https://github.com/PaesslerAG/django-httpxforwardedfor/graphs/contributors
