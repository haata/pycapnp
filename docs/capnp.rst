.. _api:

API Reference
=============

.. automodule:: capnp

.. currentmodule:: capnp


Classes
-------

RPC
~~~

Promise
#######

.. autoclass:: Promise
  :members:
  :undoc-members:
  :inherited-members:

Promise may be one of:

* :meth:`capnp.lib.capnp._Promise`
* :meth:`capnp.lib.capnp._RemotePromise`
* :meth:`capnp.lib.capnp._VoidPromise`
* :meth:`PromiseFulfillerPair`

.. autoclass:: capnp.lib.capnp._Promise
  :members:
  :undoc-members:
  :inherited-members:

.. autoclass:: capnp.lib.capnp._RemotePromise
  :members:
  :undoc-members:
  :inherited-members:

TODO

.. autoclass:: capnp.lib.capnp._VoidPromise
  :members:
  :undoc-members:
  :inherited-members:

.. autoclass:: PromiseFulfillerPair
  :members:
  :undoc-members:
  :inherited-members:


Communication
#############

.. autoclass:: TwoPartyClient
  :members:
  :undoc-members:
  :inherited-members:

TODO

.. autoclass:: TwoPartyServer
  :members:
  :undoc-members:
  :inherited-members:

TODO


Capability
##########

.. autoclass:: capnp.lib.capnp._DynamicCapabilityClient
  :members:
  :undoc-members:
  :inherited-members:

TODO


Response
########

.. autoclass:: capnp.lib.capnp._Response
  :members:
  :undoc-members:
  :inherited-members:

TODO


Miscellaneous
~~~~~~~~~~~~~
.. autoclass:: KjException
  :members:
  :undoc-members:
  :inherited-members:

TODO

.. autoclass:: SchemaParser
  :members:
  :undoc-members:
  :inherited-members:

TODO


Functions
---------
.. autofunction:: add_import_hook
.. autofunction:: cleanup_global_schema_parser
.. autofunction:: create_event_loop
.. autofunction:: getTimer
.. autofunction:: join_promises
.. autofunction:: load
.. autofunction:: poll_once
.. autofunction:: remove_event_loop
.. autofunction:: remove_import_hook
.. autofunction:: reset_event_loop
.. autofunction:: wait_forever


Internal Classes
----------------
These classes are internal to the library. You will never need to allocate
one yourself, but you may end up using some of their member methods.

Modules
~~~~~~~
These are classes that are made for you when you import a Cap'n Proto file::

  import capnp
  import addressbook_capnp

  print type(addressbook_capnp.Person) # capnp.capnp._StructModule

.. autoclass:: _InterfaceModule
  :members:
  :undoc-members:
  :inherited-members:

.. autoclass:: _StructModule
  :members:
  :undoc-members:
  :inherited-members:

Readers
~~~~~~~
.. autoclass:: _DynamicListReader
  :members:
  :undoc-members:
  :inherited-members:

.. autoclass:: _DynamicStructReader
  :members:
  :undoc-members:
  :inherited-members:

.. autoclass:: _PackedFdMessageReader
  :members:
  :undoc-members:
  :inherited-members:

.. autoclass:: _StreamFdMessageReader
  :members:
  :undoc-members:
  :inherited-members:

Builders
~~~~~~~~
.. autoclass:: _DynamicResizableListBuilder
  :members:
  :undoc-members:
  :inherited-members:

.. autoclass:: _DynamicListBuilder
  :members:
  :undoc-members:
  :inherited-members:

.. autoclass:: _DynamicStructBuilder
  :members:
  :undoc-members:
  :inherited-members:

.. autoclass:: _MallocMessageBuilder
  :members:
  :undoc-members:
  :inherited-members:

RPC
~~~
.. autoclass:: _CapabilityClient
  :members:
  :undoc-members:
  :inherited-members:

.. autoclass:: _DynamicCapabilityClient
  :members:
  :undoc-members:
  :inherited-members:

Miscellaneous
~~~~~~~~~~~~~
.. autoclass:: _DynamicOrphan
  :members:
  :undoc-members:
  :inherited-members:
