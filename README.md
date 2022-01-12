# JAR Relocator
Fork of lucko's [jar-relocator](https://github.com/lucko/jar-relocator) used by my plugins that require external/additional libraries to work.
There are just two differences with the original version: it should avoid loading libraries' classes that do not work with the current Java version (see [Java 9's multi-release JAR files](https://docs.oracle.com/javase/9/docs/specs/jar/jar.html#Multi-release)) by simply ignoring them and, obviously, the package name is changed so that the JAR gets loaded even if the original version's classpath is loaded already.
