=============================
cookiecutter-opentelekomcloud
=============================

Cookiecutter template for an Open Telekom Cloud project. See https://github.com/audreyr/cookiecutter.

* Free software: Apache license
* pbr_: Set up to use Python Build Reasonableness
* hacking_: Enforces the OpenStack Hacking Guidelines
* stestr_: Runs tests using stestr
* OpenTelekomCloud-Infra_: Ready for OpenTelekomCloud Continuous Integration testing
* Tox_ testing: Setup to easily test for Python 3.7
* Sphinx_ docs: Documentation ready for generation and publication

Usage
-----

Install cookiecutter::

    pip install cookiecutter

Generate a Python package project::

    cookiecutter https://github.com/opentelekomcloud/cookiecutter.git

OpenTelekomCloud projects require a working git repo for pbr to work, on newer
versions of cookiecutter (>= 0.7.0 released 2013-11-09) this initial commit will
be done automatically. Otherwise you will need to init a repo and commit to it
before doing anything else::

    cd $repo_name
    git init
    git add .
    git commit -a

Then:

* Add the project to the OpenTelekomCloud Infrastructure


.. _pbr: https://docs.openstack.org/pbr/latest/
.. _stestr: https://stestr.readthedocs.io/
.. _Tox: https://tox.readthedocs.io/en/latest/
.. _Sphinx: https://www.sphinx-doc.org/en/master/
.. _hacking: https://opendev.org/openstack/hacking/
