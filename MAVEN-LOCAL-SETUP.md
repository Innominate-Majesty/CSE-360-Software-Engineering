# Local Maven workspace

This Maven structure is a local development wrapper around the original Eclipse homework projects.
It does not alter or place build output inside any homework directory.

## Commands

Run all commands from this course folder with Java 25 selected.

```bash
export JAVA_HOME=$(/usr/libexec/java_home -v 25)
export PATH="$JAVA_HOME/bin:$PATH"
```

Compile every current project:

```bash
./mvnw compile
```

Run Foundations with JavaFX and H2:

```bash
./mvnw -pl maven-modules/foundations compile javafx:run
```

Run the password evaluation GUI:

```bash
./mvnw -pl maven-modules/password-evaluation compile javafx:run
```

Run the username recognizer:

```bash
./mvnw -pl maven-modules/username-recognizer compile exec:java
```

Run the finite-state-machine system:

```bash
./mvnw -pl maven-modules/finite-state-machine compile exec:java
```

Maven output is written only beneath `maven-modules/*/target`.
