# Maven VS Ant

Two examples of the same HelloWorld application with the scripting tool Ant and
the build tool Maven.

Check at my [Blog](http://coderade.in) an article that I created showing some
differences between the tools Maven and Ant tool in English and Portuguese:

* [Ant VS Maven - English](http://coderade.in/ant-vs-maven)
* [Ant VS Maven - Portuguese](http://br.coderade.in/ant-vs-maven)

### Running the Ant example

#### Install

To run the Ant example you need to have the [Ant](http://ant.apache.org/) tool installed.
To help you install this tool, look the file [INSTALL.md](../INSTALL.md).

#### Running

To compile, package and run the application you can use the commands:

```
ant compile
ant jar
ant run
```

### Running the Maven example

#### Install

To run the Maven example you need to have the [Maven](https://maven.apache.org) tool installed.
To help you install this tool look the file [INSTALL.md](../INSTALL.md).

#### Running

To run this example you can use the commands:

`mvn clean` - that's will clear any compiled files you have,
making sure that you're really compiling each module from scratch

`mvn compile` - that's will compile the source code of the project.

After run the `compile` command, a ***target*** directory will be created.

So can use the command `cd target/classes` and run the command:

`java main.java.HelloWorld`

to run the application.
