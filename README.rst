
restible-flask
##############

.. readme_inclusion_marker

**restible-flask** is a library that provides **Flask** integration with
`restible <https://github.com/novopl/restible>`_. It provides the base endpoint
class ``FlaskEndpoint`` that that integrates
`restible <https://github.com/novopl/restible>`_ with Flask routing.


.. note::
    The CircleCI builds can be found
    `here <https://circleci.com/gh/novopl/restible-flask>`_

Installation
============

.. code-block:: shell

    $ pip install restible-flask


Contributing
============

Setting up development repo
---------------------------

.. code-block:: shell

    $ git clone git@github.com:novopl/restible-flask.git
    $ cd restible-flask
    $ virtualenv env
    $ source ./env/bin/activate
    $ python setup.py develop
    $ pip install -r ops/devrequirements.txt
    $ peltak git add-hooks


Running tests
.............

**Config**: The types of tests are defined in ``pelconf.py`` and the
pytest configuration is defined in ``ops/tools/pytest.ini``.

.. code-block:: shell

    $ peltak test

Linting
.......

**Config**: The list of locations to lint is defined in ``pelconf.py`` and the
linters configuration is defined in ``ops/tools/{pylint,pep8}.ini``.

.. code-block:: shell

    $ peltak lint

Generating docs
...............

**Config**: The list of documented files and general configuration is in
``pelconf.py`` and the Sphinx configuration is defined in ``docs/conf.py``.

.. code-block:: shell

    $ peltak docs
