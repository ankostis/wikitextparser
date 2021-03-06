v0.22.1
-------
- Fixed MemoryError caused by very long or unclosed comment tags (issue #12)

v0.22.0
-------
- Change the behaviour of external_links property to never return Templates or parser functions as part of the external link.
- Add support for literal IPv6 external links, e.g. https://[2001:db8:85a3:8d3:1319:8a2e:370:7348]:443/.
- Fixed: Do not mistake the equal signs of section titles for template keyword arguments.

v0.21.5
-------
- Fixed Invalid escape sequences for Python 3.6.
- Added ``msg``, ``msgnw``, ``raw``, ``safesubst``, and ``subst`` to known parser function identifiers.

v0.21.4
-------
- Fixed a bug in Table.data (issue #9)

v0.21.3
-------
- Fixed: A bug in processing ``Section`` objects.

v0.21.2
-------
- Fixed: A bug in ``external_links`` (the starting position must now be a word boundary; previously this condition was not checked)

v0.21.1
-------
- Fixed: A bug in ``external_links`` (external links withing sub-templates are now detected correctly; previously they were ignored)

v0.21.0
-------
- Changed: The order of results, now everything is sorted by its starting position.
- Fixed: Bug in ``ancestors`` and ``parent`` methods

v0.20.0
-------
- Added: ``parent`` and ``ancestors`` methods
- Added: ``__version__`` to ``__init__.py``

v0.19.0
-------
- Removed: Support for Python 3.3
- Fixed: Handling of comments and tags in section titles

v0.18.0
-------
- Changed: Add an underscore prefix to private internal modules names
- Changed: Moved test modules to a different directory
- Changed: Templates adjacent to external links are now treated as part of the link
- Fixed: A bug in handling tag extensions withing parser functions
- Fixed: A minor bug in Template.set_arg
- Changed: ExternalLink.text: Return None if the link is not within brackets
- Fixed: Handling of comments and templates in external links
