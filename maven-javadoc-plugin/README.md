# Maven Javadoc Plugin

This example show how to use the java docs plugin inside a Maven POM file.

## The Javadoc Plugin

The Javadoc Plugin uses the Javadoc tool to generate javadocs for the specified project.


The Javadoc plugin is almost identical to the source plugin in the sense that it's going to take our Javadocs and package them to our jar file when we upload them to our repository. The Javadoc plugin is also tied to the package phase, but if we're running package a lot of it can hinder performance so we'll override it to like the verify phase.

Usually, we just use the defaults but if you have customized Javadocs for your company before, maybe throw in your company logo on there, or change colors, or whatever, you can customize all that inside this Javadoc plugin.

If we were to do some of those customizations that I mentioned earlier for the Javadoc, we would do that inside of a configuration section.

## About the example

In this example I added another plugin section inside of our build element and added the three things that we need, our groupId, artifactId, and version number. The artifactId is maven-javadoc-plugin, and then our version is 2.10.3. If you want to customize things like color, that type of stuff, you would want to specify a configuration section as well.

I set the id to call attach-javadocs and the phase, I changed the default that was package to the verify phase because I want it to run just before I install it and deploy it, and then I'll add a goal for it to run on as well in case I have to run the jar goal by itself. I'll tie it to that as well so there's our jar.


For more information about the Javadoc plugin check this link: [Apache Maven Source Plugin](https://maven.apache.org/plugins/maven-javadoc-plugin/).

### Installing Maven

To run this example you need to install the Maven. Check the file [INSTALL.md](../INSTALL.md).


### Running

To run this example you can use the command your command line:

`mvn install` - this command will go through and make sure that our code is all up to date, everything is compiled, and then it will take and download the sources plugin if I don't already have it installed, and build those sources for it.

After run this command you'll see it attached the source and it generated our Javadocs. See all this code piling out here is where it's coming out and creating our API docs folder for us and building the package frame and values, and all classes and all that information. Then I went ahead and uploaded those all to our repository so we have our source code getting uploaded, our sources, and then our Javadocs.

So you can go in the `target/apidocs` directory you'll see all HTML files of your Javadoc created.
