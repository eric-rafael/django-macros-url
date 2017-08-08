v0.4.0
------

Added Py3.{5,6} & Django 1.11. Removed Py2.6 & Django <1.8 (#9)
* Quick fix for the DJANGO_VERSION error when using Python >= 3.6 (version calculation caching removed because it is not a performance penalty, urls are lazy and are calculated only once per an app start).

* Added Py3.{5,6} & Django 1.11. Removed Py2.6 & Django <1.8

The latest Django LTS is 1.11. Its ok to support up to the "LTS -1" (1.8) only.
The next Django LTS is 2.0, and will be Py3k only, so lets start testing with Py3k!

* Mark as Py3k compat on setup.py

v0.3.1
------

Fix for https://github.com/phpdude/django-macros-url/issues/8.

v0.3.0
------

Added support for Django 1.10 version.

v0.2.3
------

Development Status changed to "Development Status :: 5 - Production/Stable".

v0.2.2
------

Reverting tests back.

v0.2.1
------

Added `django.setup()` for tests, because looks like now it is required. README.markdown fixes.

v0.2.0
------

Added auto-calling as_view on CBVs objects. Now you can omit as_view() in your views by default. 
Have your code more clean then before ;-)

v0.1.7
------

setup.py fixes in requires.

v0.1.6
------

Tests updated to support Django1.8. Travis configuration updated too. Small cleanups.

v0.1.5
------

Add uuid version to uuid regex

v0.1.4
------

Readme fixes.

v0.1.3
------

macrosurl.__init__ django import fix to allow install macros-url when django is not installed yet.

v0.1.2
------

added pk macros

v0.1.1
------

Support for include('path.to.url') view added. Urls normalization by adding dollar at end fixed to support include. Tests added.

v0.1.0
------

Basic functionality done.