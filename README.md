AcmeFetch
=========
Version: #VERSION#
Date: #DATE#

AcmeFetch is a thin wrapper arount he ACME::Protocol library to fetch and maintain
ssl certificates using the the services of Let's Encrypt!

Setup
-----
Now got back to your app source directory start building

 ./configure --prefix=$HOME/opt/acmefetch
 make

Configure will check if all requirements are met and give
hints on how to fix the situation if something is missing.

Any mising perl modules will be built and installed into the prefix
directory. Your system perl will NOT be affected by this.

Installation
------------

To install the application, just run

   make install

Packaging
---------

Before release, make sure to update CHANGES, VERSION and run ./bootstrap

You can also package the application as a nice tar.gz file, it will contain
a mini copy of cpan, so that all perl modules can be rebuilt at the
destination.  If you want to make sure that your project builds with perl
5.10.1, make sure to set the PERL environment variable to a perl 5.10.1 interpreter,
make sure to delete any PERL5LIB environment variable, remove the thirdparty
directory from your source tree and configure again.  Now all modules to build your
project with any perl from 5.10.1 on upward will be included in the distribution.

   make dist

Enjoy!

Tobias Oetiker <tobi@oetiker.ch>