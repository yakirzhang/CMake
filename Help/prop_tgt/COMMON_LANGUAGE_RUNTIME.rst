COMMON_LANGUAGE_RUNTIME
-----------------------

By setting this target property, the target is configured to build with
``C++/CLI`` support.

The Visual Studio generator defines the ``clr`` parameter depending on
the value of ``COMMON_LANGUAGE_RUNTIME``:

* property not set: native C++ (i.e. default)
* property set but empty: mixed unmanaged/managed C++
* property set to any non empty value: managed C++

Supported values: ``""``, ``"pure"``, ``"safe"``

This property is only evaluated :ref:`Visual Studio Generators` for
VS 2010 and above.

See also :prop_tgt:`IMPORTED_COMMON_LANGUAGE_RUNTIME`
