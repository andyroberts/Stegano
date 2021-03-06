Release History
===============

0.6.1 (2016-08-25)
------------------

* reorganization of the steganalysis sub-module.

0.6 (2016-08-04)
------------------

* improvements of the command line of Stéganô. The use of Stéganô through the
  command line has slightly changed ('hide' and 'reveal' are now sub-parameters
  of the command line). No changes if you use Stéganô as a module in your
  software. The documentation has been updated accordingly.

0.5.5 (2016-08-03)
------------------

* bugfix: Incorrect padding size in `base642string` in tools.base642binary().

0.5.4 (2016-05-22)
------------------

* the generator provided to the functions lsbset.hide() and lsbset.reveal() is
  now a function. This is more convenient for a user who wants to use a custom
  generator (not in the module lsbset.generators).
* performance improvements for the lsb and lsbset modules.

0.5.3 (2016-05-19)
------------------

* reorganization of all modules. No impact for the users of Stegano.

0.5.2 (2016-05-18)
------------------

* improvements and bug fixes for the exifHeader module;
* added unit tests for the exifHeader module;
* improvements of the documentation.

0.5.1 (2016-04-16)
------------------

* minor improvements and bug fixes;
* added unit tests for the slsb and slsbset modules.

0.5 (2016-03-18)
----------------

* management of greyscale images.

0.4.6 (2016-03-12)
------------------

* bugfix when the length of the message to hide is not divisible by 3,
  for the slsb and slsbset module.

0.4.5 (2015-12-23)
------------------
* bugfix.

0.4.4 (2015-12-23)
------------------

* new project home page;
* minor updated to the documentation.

0.4.3 (2015-10-06)
------------------

* bug fixes for Python 3;
* bug fixes in the scripts in *./bin*.

0.4.2 (2015-10-05)
------------------

* first stable release on PypI.

0.4 (2012-01-02)
----------------

This release introduces a more advanced LSB (Least Significant Bit) method
based on integers sets. The sets generated with Python generators
(Sieve of Eratosthenes, Fermat, Carmichael numbers, etc.) are used to select
the pixels used to hide the information. You can use these new methods in your
Python codes as a Python module or as a program in your scripts.

0.3 (2011-04-15)
----------------

* you can now use Stéganô as a library in your Python program;
  (python setup.py install) or as a 'program' thanks to the scripts provided
  in the bin directory;
* new documentation (reStructuredText) comes with Stéganô.

0.2 (2011-03-24)
----------------

* this release introduces some bugfixes and a major speed improvement of the
  *reveal* function for the LSB method. Moreover it is now possible to hide a
  binary file (ogg, executable, etc.);
* a new technique for hiding/revealing a message in a JPEG picture by using the
  description field of the image is provided.
