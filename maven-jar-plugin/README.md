# Maven Jar Plugin

This example show how to use the jar plugin inside a Maven POM file.

## The Jar Plugin

This plugin provides the capability to build jars.

In this example I set the value of the **useDefaultManifestFile**
to *true* to enable the compile command to create a default [Manifest File](https://docs.oracle.com/javase/tutorial/deployment/jar/manifestindex.html).

For more information about the Compiler plugin check this link: [Apache Maven Jar Plugin](https://maven.apache.org/plugins/maven-jar-plugin/).

### Installing Maven

To run this example you need to install the Maven. Check the file [INSTALL.md](../INSTALL.md).


### Running

To run this example you can use the commands:

`mvn clean` - that's will clear any compiled files you have,
making sure that you're really compiling each module from scratch.

`mvn compile` - that's will compile the source code of the project.

After run the `compile` command, a ***target*** directory will be created.

So can use the command `cd target/classes` and run the command:

```
java main.java.HelloWorld
```

to run the application.
