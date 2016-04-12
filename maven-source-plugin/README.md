# Maven Source Plugin

This example show how to use the jar plugin inside a Maven POM file.

## The Source Plugin

The Source Plugin creates a jar archive of the source files of the current project. The jar file is, by default, created in the project's target directory.


The Source Plugin can often be confusing to people because they think it's for doing something more with our source code and actually it's used to attach our source code to a jar. So you've seen as we've been browsing some of the sites that we've looked at that they'll have source code available for us to look at when we inside of our IDE so as if we're debugging something or stepping through something, we have source code available to step into. That's what this plugin does is it generates our source code for us in a jar so we can upload it to the repository.

It is tied by default to the package phase and frequently overridden to a later phase. If you're running package a lot, you don't want to sit there and wait for it. So a lot of people wait until they tie it to the install phase or even the deploy phase just because it's slowing their build down.

## About the example

In this example I've defined a plugin that I've changed it to use the verify phase, this run right before the install and deploy phase.

For more information about the Compiler plugin check this link: [Apache Maven Source Plugin](https://maven.apache.org/plugins/maven-source-plugin/).

### Installing Maven

To run this example you need to install the Maven. Check the file [INSTALL.md](../INSTALL.md).


### Running

To run this example you can use the command your command line:

`mvn install` - this command will go through and make sure that our code is all up to date, everything is compiled, and then it will take and download the sources plugin if I don't already have it installed, and build those sources for it. And if you notice in you command line, it says that it's attaching the sources right here, that's our ID that's why I put in this example (Look the pom.xml file). We always need to give it a good ID that makes sense so that we can and when we're running our application, we can tell from the logs that are rolling off the screen what's actually happening.
