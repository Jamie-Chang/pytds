pytds
=====

![Build Status](https://secure.travis-ci.org/denisenkom/pytds.png?branch=master)
   

Python DBAPI driver for MSSQL using pure Python TDS (Tabular Data Stream) protocol implementation

It can be used with https://bitbucket.org/denisenkom/django-pytds as a django database backend.

Features
--------

* Fully supports new MSSQL 2008 date types: datetime2, date, time, datetimeoffset
* MARS

Missing Features
----------------

* SSL encryption

Installation
------------

To install run this command:

    pip install python-tds

For a better performance install bitarray package too:

    pip install bitarray

Example
-------

To connect to database do
    
    import pytds
    conn = pytds.connect('server', 'database', 'user', 'password')

For the api reference see [DBAPI Specification](http://legacy.python.org/dev/peps/pep-0249/)
