# checker-gradle-demo
Demo of Gradle app using the Java Checker Framework

The Gradle script contains a task called `resolveAnnotatedJdk` which you can run to ensure the jar was found
in Maven Central.

To see where it is resolved locally, run:

```
./gradlew resolveAnnotatedJdk --INFO
```

All declared dependencies are for the [Checker Framework](http://checkerframework.org).

The only declared checker is the NullnessChecker.

Running `./gradlew clean compileJava` will compile the Java code using the Checker Framework checkers.