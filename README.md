<h1><img src="https://github.com/brettwooldridge/HikariCP/wiki/Hikari.png"> HikariCP<sup><sup>&nbsp;It's Faster.</sup></sup><sub><sub><sup>Hi·ka·ri [hi·ka·'lē] &#40;<i>Origin: Japanese</i>): light; ray.</sup></sub></sub></h1><br>

# HikariCP Fork with Virtual Thread Support

This repository contains a fork of HikariCP that includes changes from merge request [#2055](https://github.com/brettwooldridge/HikariCP/pull/2055) to add support for Java 21 virtual threads.

## Overview

HikariCP is a solid, high-performance JDBC connection pool. This fork specifically integrates a proposed enhancement to support Java's virtual thread model introduced in Java 21, making it suitable for applications leveraging the new concurrency model in Java.

## Compatibility

- **Java Version**: This version of HikariCP is compatible only with **Java 21** and above due to its reliance on virtual threads.
- **Database Compatibility**: It maintains compatibility with databases supported by the original HikariCP.

## Future Transition to Official Release

It is anticipated that future releases of Java, specifically Java 23, will address the current issues with virtual thread pinning at synchronized blocks ([more information about the issue could be found here](https://mail.openjdk.org/pipermail/loom-dev/2024-February/006433.html)). Once these improvements are implemented, users are encouraged to transition back to the official release of HikariCP. This would ensure compatibility with the latest Java standards and security enhancements, along with receiving ongoing support and updates from the HikariCP community.

Stay tuned to the [official HikariCP repository](https://github.com/brettwooldridge/HikariCP) and Java release notes for updates on these changes. Using the official release is recommended as soon as it fully supports the enhanced concurrency model of Java 23 and beyond.
