# Maven with Repositories Example

This example use some repositories and the snapshot and release section.

## Repositories

The repositories might be a truly remote repository set up by a third party to provide their artifacts for
downloading (for example, repo.maven.apache.org and uk.maven.org house Maven's central repository).
Other "remote" repositories may be internal repositories set up on a file or HTTP server within your company,
used to share private artifacts between development teams and for releases.

## `<snapshot/>` and `<release/>` tags
These sections are the policies for each type of artifact, Release or snapshot.
With these two sets, a POM has the power to alter the policies for each type independent of the other within a single repository.

## About the example

For the example, I  decide to enable only snapshot downloads for development purposes.

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
