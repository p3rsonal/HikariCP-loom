<h1><img src="https://github.com/brettwooldridge/HikariCP/wiki/Hikari.png"> HikariCP<sup><sup>&nbsp;It's Faster.</sup></sup><sub><sub><sup>Hi·ka·ri [hi·ka·'lē] &#40;<i>Origin: Japanese</i>): light; ray.</sup></sub></sub></h1><br>

# HikariCP Fork with Virtual Thread Support

This repository contains a fork of HikariCP that includes changes from merge request [#2055](https://github.com/brettwooldridge/HikariCP/pull/2055) to add support for Java 21 virtual threads.

## Overview

HikariCP is a solid, high-performance JDBC connection pool. This fork specifically integrates a proposed enhancement to support Java's virtual thread model introduced in Java 21, making it suitable for applications leveraging the new concurrency model in Java.

## Compatibility

- **Java Version**: This version of HikariCP is compatible only with **Java 21** and above due to its reliance on virtual threads.
- **Database Compatibility**: It maintains compatibility with databases supported by the original HikariCP.
