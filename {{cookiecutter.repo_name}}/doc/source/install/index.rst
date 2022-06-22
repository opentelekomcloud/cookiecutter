{%- macro set_header_markup(header_text_length) -%}
{%- for _ in range(0, header_text_length) -%}={%- endfor -%}
{%- endmacro -%}
{%- macro set_header(header_text) -%}
{{ set_header_markup(header_text|length) }}
{{header_text}}
{{ set_header_markup(header_text|length) }}
{%- endmacro -%}
{{ set_header(" {{cookiecutter.module_name}} installation guide") }}

.. toctree::
   :maxdepth: 2

   install.rst

The {{cookiecutter.module_name}} provides...

This chapter assumes a working setup of OpenStack following the
`OpenStack Installation Tutorial
<https://docs.openstack.org/project-install-guide/ocata/>`_.
