galaxy-bootstrap
================

[![Build Status](https://travis-ci.org/jmchilton/galaxy-bootstrap.png?branch=master)](https://travis-ci.org/jmchilton/galaxy-bootstrap)

galaxy-boostrap is a small Java library allowing for programmatic
download and configuration of the [Galaxy
framework](http://galaxyproject.org). The initial goal of this project
is to be used for the automated testing of
[blend4j](http://github.com/jmchilton/blend4j), but it may have some
interesting applications (when paired with blend4j) in terms of using
Galaxy as computational platform within the context of a JVM
application.

### Requirements

- Java 6
- Maven 
- Mercurial

### Logging

Logging is provided by [log4j](http://logging.apache.org/log4j/1.2/index.html).  Additional information can be displayed by setting the level from `INFO` to `DEBUG` within [src/main/resources/log4j.properties](src/main/resources/log4j.properties) or by passing a new properties file on the command line.  For example:

```bash
cp src/main/resources/log4j.properties ./
mvn test -Dlog4j.configuration=file:./log4j.properties
```
