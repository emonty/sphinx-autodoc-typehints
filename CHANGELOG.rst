1.2.1
=====

* Fixed `ValueError` when `getargspec()` encounters a built-in function
* Fixed `AttributeError` when `Any` is combined with another type in a `Union`
  (thanks Davis Kirkendall)


1.2.0
=====

* Fixed compatibility with Python 3.6 and 3.5.3
* Fixed ``NameError`` when processing signatures of wrapped functions with type hints
* Fixed handling of slotted classes with no ``__init__()`` method
* Fixed Sphinx warning about parallel reads
* Fixed return type being added to class docstring from its ``__init__()`` method
  (thanks to Manuel Krebber for the patch)
* Fixed return type hints of ``@property`` methods being omitted (thanks to pknight for the patch)
* Added a test suite (thanks Manuel Krebber)


1.1.0
=====

* Added proper support for ``typing.Tuple`` (pull request by Manuel Krebber)


1.0.6
=====

* Fixed wrong placement of ``:rtype:`` if a multi-line ``:param:`` or a ``:returns:`` is used


1.0.5
=====

* Fixed coroutine functions' signatures not being processed when using sphinxcontrib-asyncio


1.0.4
=====

* Fixed compatibility with Sphinx 1.4


1.0.3
=====

* Fixed "self" parameter not being removed from exception class constructor signatures
* Fixed process_signature() erroneously removing the first argument of a static method


1.0.2
=====

* Fixed exception classes not being processed like normal classes


1.0.1
=====

* Fixed errors caused by forward references not being looked up with the right globals


1.0.0
=====

* Initial release
