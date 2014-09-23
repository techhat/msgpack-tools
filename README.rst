msgpack Tools
=============

``msgpack`` has become a popular serialization tool, especially with common use
in the SaltStack suite of tools. As a developer, I frequently have a need to
look inside or even edit ``msgpack`` files. These are little tools that I have
developed in order to help me out.

packcat
-------
The ``packcat`` command emulates the ``cat`` command, after translating the
file in question to a Python dictionary. The dictionary is sent to the user via
the ``pprint`` library.

packedit
--------
The ``packedit`` command will read a ``msgpack``-encoded file, convert it to
JSON, and open it for editing in the ``EDITOR`` that is defined in the
shell environment. If no ``EDITOR`` is set, ``vim`` is used by default.
