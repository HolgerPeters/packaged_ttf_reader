# FOP Helper

An executable jar for converting ttf fonts to Apache FOP
metric files.

## Why?

Apache FOP offers the org.apache.fop.fonts.apps.TTFReader
tool for extracting metadata from TTF file that FOP needs to
use them in pdf generation. Unfortunately, running TTFReader
involves a lot of classpath fighting.

This small Java project bundles TTFReader and all necessary
dependencies into a single jar using `mvn clean compile
assembly:single`, that you can directly execute with `java
-jar`.


