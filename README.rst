msgpack Tools
=============

``msgpack`` has become a popular serialization tool, especially with common use
in the SaltStack suite of tools. As a developer, I frequently have a need to
look inside or even edit ``msgpack`` files. These are little tools that I have
developed in order to help me out.

packcat
-------
The ``packcat`` command emulates the ``cat`` command, after translating the
file in question to a Python dictionary. The dictionary is displayed to the user
in JSON format.

packedit
--------
The ``packedit`` command will read a ``msgpack``-encoded file, convert it to
JSON, and open it for editing in the ``EDITOR`` that is defined in the
shell environment. If no ``EDITOR`` is set, ``vim`` is used by default.

packdiff
--------
The ``packdiff`` command will read two ``msgpack``-encoded files, convert them
to JSON, and open them for editing in the ``DIFFTOOL`` that is defined in the
shell environment. If no ``DIFFTOOL`` is set, ``vimdiff`` is used by default.
