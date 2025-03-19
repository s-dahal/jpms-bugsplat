# test
This repository contains a Java Platform Module System (JPMS) compliant version of the ANTLR4 runtime library. The goal of this project is to provide a modularized version of the ANTLR4 runtime that can be easily integrated into Java projects using JPMS.

## Features

* **JPMS Compliance:** The library is packaged as a JPMS module, enabling better encapsulation and dependency management in Java projects.
* **Ease of Use:** Simple integration into projects using JPMS.

## Getting Started
### Prerequisites

* **Java 11 or higher:** JPMS was introduced in Java 9, so a minimum of Java 11 is recommended for compatibility and support.
* **Maven or Gradle:** For dependency management and building the project.

Add the following dependency to your pom.xml:
```xml
<dependency>
    <groupId>dev.ikm.jpms</groupId>
	<artifactId>antlr4-runtime</artifactId>
    <version>${latest-version}</version>
</dependency>
```

Add the following dependency to your build.gradle:
```groovy
implementation 'dev.ikm.jpms:antlr4-runtime:${latest-version}'
```

In your module descriptor (module-info.java), declare the dependency on the antlr4.runtime module:

```java
module your.module.name {
    requires dev.ikm.jpms.antlr4.runtime;
}
```


## Issues and Contributions
Technical and non-technical issues can be reported to the [Issue Tracker](https://github.com/ikmdev/repo-seed/issues).

Contributions can be submitted via pull requests. Please check the [contribution guide](doc/how-to-contribute.md) for more details.