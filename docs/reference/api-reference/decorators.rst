========================
Decorators
========================
While the 1:1 mapping of output -> function implementation is powerful, we've implemented a few decorators to promote
business-logic reuse. Source for these decorators can be found in the
`function_modifiers module <https://github.com/dagworks-inc/hamilton/blob/main/hamilton/function_modifiers>`__.

For reference we list available decorators for Hamilton here. Note: use
``from hamilton.function_modifiers import DECORATOR_NAME`` to use these decorators:

@config*
------------------------
.. autoclass:: hamilton.function_modifiers.config
   :members: when, when_in, when_not, when_not_in
   :special-members: __init__


@tag*
------------------------
.. autoclass:: hamilton.function_modifiers.tag
   :special-members: __init__

.. autoclass:: hamilton.function_modifiers.tag_outputs
   :special-members: __init__


@extract*
------------------------
.. autoclass:: hamilton.function_modifiers.extract_columns
   :special-members: __init__

.. autoclass:: hamilton.function_modifiers.extract_fields
   :special-members: __init__


@check\_output*
------------------------
.. autoclass:: hamilton.function_modifiers.check_output
   :special-members: __init__

.. autoclass:: hamilton.function_modifiers.check_output_custom
   :special-members: __init__


@parameterize*
------------------------
Classes to help with @parameterize:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. autoclass:: hamilton.function_modifiers.ParameterizedExtract

.. autoclass:: hamilton.function_modifiers.source

.. autoclass:: hamilton.function_modifiers.value

.. autoclass:: hamilton.function_modifiers.group


Actual decorators:
^^^^^^^^^^^^^^^^^^^^^^^^^

.. autoclass:: hamilton.function_modifiers.parameterize
   :special-members: __init__

.. autoclass:: hamilton.function_modifiers.parameterize_sources
   :special-members: __init__

.. autoclass:: hamilton.function_modifiers.parameterize_values
   :special-members: __init__

.. autoclass:: hamilton.function_modifiers.parameterize_extract_columns
   :special-members: __init__

.. autoclass:: hamilton.experimental.decorators.parameterize_frame.parameterize_frame
   :special-members: __init__

@inject
------------------------
.. autoclass:: hamilton.function_modifiers.inject
   :special-members: __init__

@does
------------------------
.. autoclass:: hamilton.function_modifiers.does
   :special-members: __init__


@subdag
------------------------
.. autoclass:: hamilton.function_modifiers.subdag
   :special-members: __init__

@parameterized_subdag
------------------------
.. autoclass:: hamilton.function_modifiers.parameterized_subdag
   :special-members: __init__

@resolve
------------------------
.. autoclass:: hamilton.function_modifiers.resolve
   :special-members: __init__

@load_from
------------------------
.. autoclass:: hamilton.function_modifiers.load_from
   :special-members: __init__

@save_to
------------------------
.. autoclass:: hamilton.function_modifiers.save_to
   :special-members: __init__
