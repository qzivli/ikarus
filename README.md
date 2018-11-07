# Ikarus Scheme

Ikarus Scheme is an implementation of the Scheme programming language.  The preliminary release of Ikarus implements the majority of the features found in the current standard, the Revised 6 report on the algorithmic language Scheme including full R6RS library and script syntax, syntax-case, unicode strings, bytevectors, user-defined record types, exception handling, conditions, and enumerations.  Over 80% of the R6RS procedures and keywords are currently implemented and subsequent releases will proceed towards brining Ikarus to full R6RS conformance.

The main purpose behind releasing Ikarus early is to give Scheme programmers the opportunity to experiment with the various new features that were newly introduced in R6RS.  The most important of such features is the ability to structure large programs into libraries; where each library extends the language through procedural and syntactic abstractions.  Many useful libraries can be written using the currently supported set of R6RS features including text processing tools, symbolic logic systems, interpreters and compilers, and many mathematical and scientific packages.  It is my hope that this release will encourage the Scheme community to write and to share their most useful R6RS libraries.


## This repository

This repository contains source codes and prebuilt binaries of Ikarus Scheme version 0.0.4-rc1+ (revision 1870).


## Installation

### macOS

Modify the version number according to your situation.
```
brew install libffi

./configure --enable-libffi \
    CFLAGS=-I/usr/local/Cellar/libffi/3.2.1/lib/libffi-3.2.1/include \
    LDFLAGS=-L/usr/local/Cellar/libffi/3.2.1/lib

make 
sudo make install
```

Note: this will install `/usr/local/bin/scheme-script`, may overwrite the Chez Scheme one.


### GNU/Linux

TBD


## The Scheme Programming Language

For more information about the Scheme programming language, see:

* [The Revised^6 Report on the Algorithmic Language Scheme](http://www.r6rs.org)
* [The Scheme Programming Language (fourth edition), by R. Kent Dybvig](https://www.scheme.com/tspl4/)
* [The Little Schemer](https://mitpress.mit.edu/books/little-schemer-fourth-edition)
* [The Little Schemer 中文版](https://book.douban.com/subject/27080946/)

