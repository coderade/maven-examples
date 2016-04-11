# Maven Hello World Example

This example show how to use the compiler plugin inside a Maven POM file.

## The Compile Plugin

The Compiler Plugin is used to compile the sources of your project. Since 3.0, the default compiler is javax.tools.JavaCompiler (if you are using java 1.6) and is used to compile Java sources. If you want to force the plugin using javac, you must configure the plugin option forceJavacCompilerUse.

Also note that at present the default source setting is 1.5 and the default target setting is 1.5, independently of the JDK you run Maven with. In this example I change this default setting the source and target section.

For more information check this link: [Apache Maven Compiler Plugin](https://maven.apache.org/plugins/maven-compiler-plugin/).

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
