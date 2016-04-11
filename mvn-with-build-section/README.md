#Maven with the build section

To override the Maven defaults we can use the build section.
The build section is where we override things of a specific nature.

In this example, I overrided the default name of our artifact that gets produce
using the build section. So that's how we can override the final name of our application,
we also can override the directory structure about where it should look for source or where the things should get compiled to.

But for this example, there's our basic of how we override our final name of our application.

#### Running

To run this example you can use the commands:

`mvn clean` - that's will clear any compiled files you have,
making sure that you're really compiling each module from scratch

`mvn compile` - that's will compile the source code of the project.

After run the `compile` command, a ***target*** directory will be created.

So can use the command `cd target/classes` and run the command:

`java main.java.HelloWorld`

to run the application.
