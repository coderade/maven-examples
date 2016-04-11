# Maven with dependencies and scope

This example use some dependencies and the scope section.

Dependency scope is used to limit the transitivity of a dependency, and also to affect the classpath used for various build tasks.

There are 6 scopes available:

*   **compile**  
    This is the default scope, used if none is specified. Compile dependencies are available in all classpaths of a project. Furthermore, those dependencies are propagated to dependent projects.
*   **provided**  
    This is much like <tt>compile</tt>, but indicates you expect the JDK or a container to provide the dependency at runtime. For example, when building a web application for the Java Enterprise Edition, you would set the dependency on the Servlet API and related Java EE APIs to scope <tt>provided</tt> because the web container provides those classes. This scope is only available on the compilation and test classpath, and is not transitive.
*   **runtime**  
    This scope indicates that the dependency is not required for compilation, but is for execution. It is in the runtime and test classpaths, but not the compile classpath.
*   **test**  
    This scope indicates that the dependency is not required for normal use of the application, and is only available for the test compilation and execution phases.
*   **system**  
    This scope is similar to <tt>provided</tt> except that you have to provide the JAR which contains it explicitly. The artifact is always available and is not looked up in a repository.
*   **import** _(only available in Maven 2.0.9 or later)_  
    This scope is only used on a dependency of type <tt>pom</tt> in the <tt><dependencyManagement></tt> section. It indicates that the specified POM should be replaced with the dependencies in that POM's <tt><dependencyManagement></tt> section. Since they are replaced, dependencies with a scope of <tt>import</tt> do not actually participate in limiting the transitivity of a dependency.

Each of the scopes (except for <tt>import</tt>) affects transitive dependencies in different ways, as is demonstrated in the table below. If a dependency is set to the scope in the left column, transitive dependencies of that dependency with the scope across the top row will result in a dependency in the main project with the scope listed at the intersection. If no scope is listed, it means the dependency will be omitted.


#### Running

To run this example you can use the commands:

`mvn clean` - that's will clear any compiled files you have,
making sure that you're really compiling each module from scratch

`mvn compile` - that's will compile the source code of the project.

After run the `compile` command, a ***target*** directory will be created.

So can use the command `cd target/classes` and run the command:

`java main.java.HelloWorld`

to run the application.
