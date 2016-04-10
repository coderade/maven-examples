# Maven Hello World Example

This a simple Hello World application using Maven.
The `pom.xml` is with all commented lines, so if you are started to learning with can use this as a example.

### Installing Maven

To run this example you need to install the Maven. Check the file [INSTALL.md](../INSTALL.md).


### Running

To run this example use the commands:

`mvn clean` - that's will clear any compiled files you have, making sure that you're really compiling each module from scratch

`mvn compile` - that's will compile the source code of the project.

After run the `compile` command, a ***target*** directory will be created.

So can use the command `cd target/classes` and run the command:

`java main.java.HelloWorld` to run the application.
