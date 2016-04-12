#Maven with dependencies

This example show how to use dependencies inside a Maven POM file.

## Dependencies

Dependencies are what we want to use inside of our application, they are imported by their naming convention.
This is often considered the most confusing part of Maven. Because we have to know what their artifact ID,
what their group ID, and what version I want to use is. The nice thing about this
though is it will pull transitive dependencies in for us.

Adding dependency to the POM file is is fairly simple, you just need to list the dependency that you want to use.
Any transitive dependencies will be pulled in for us automatically.
How this looks inside of the POM file is to just add the dependency section in at the bottom of the POM file
and add a specific dependency. Now this example here,
I'm going to show you, is to use the commons lang library which is just a library from Apache.
Nothing real exciting here.

## About the example

But just a simple example to show you how to pull in the commons lang library.
So their group ID is commons lang. Their artifact ID is also commons lang and the current version
that we were using for this example is 2.6. So this is what our POM file would now look like with that dependency in it.
There's no transitive dependencies on the commons lang module. So it's only going to download just this jar file.

#### Running

To run this example you can use the commands:

`mvn clean` - that's will clear any compiled files you have,
making sure that you're really compiling each module from scratch

`mvn compile` - that's will compile the source code of the project.

After run the `compile` command, a ***target*** directory will be created.

So can use the command `cd target/classes` and run the command:

`java main.java.HelloWorld`

to run the application.
