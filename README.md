PLV8 - A Procedural Language in Javascript powered by V8
=================================================

[![Build Status](https://travis-ci.com/heroku/plv8.svg?branch=master)](https://travis-ci.com/heroku/plv8)

PLV8 is a shared library that provides a PostgreSQL procedural language powered
by V8 Javascript Engine.  With this program you can write in Javascript your
function that is callable from SQL.

## Installing

    =# CREATE EXTENSION plv8;

This will install PLV8 into your database if it exists as an extension.

## Testing

To test, you can execute:

    =# DO $$ plv8.elog(NOTICE, "hello there!"); $$ LANGUAGE plv8;

For full documentation, see [https://plv8.github.io/](https://plv8.github.io/).
