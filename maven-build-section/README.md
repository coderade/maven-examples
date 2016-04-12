#Maven with the build section

To override the Maven defaults we can use the build section.
The build section is where we override things of a specific nature.

## About the example

In this example, I overrided the default name of our artifact that gets produce
using the build section. So that's how we can override the final name of our application,
we also can override the directory structure about where it should look for source
or where the things should get compiled to.

But for this example, there's our basic of how we override our final name of our application.

#### Running

To run this example you can use the commands:

`mvn clean` - that's will clear any compiled files you have,
making sure that you're really compiling each module from scratch

`mvn compile` - that's will compile the source code of the project.

`mvn package` - that's will create out jar package with the name change to `foo.jar`.
