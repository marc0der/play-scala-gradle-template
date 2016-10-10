# Example Play Scala Application Using Gradle

This is the Scala flavour of the existing [Java template](https://github.com/simonharrer/play-java-gradle-example) by @simonharrer.

Starting with Gradle 3.1, Play 2.5.x is (partially) supported. 
But there are no examples how to use Play 2.5.x with Gradle 3.1.
This project closes the gap by providing such an example. 

You can simply run it by executing `./gradlew -t runPlayBinary` on the command line.

## Production Deployment

Build a production deployable with `./gradlew stage`. Don't forget to change `play.crypto.secret` in the `conf/application.conf` before building the deployable.

## Changes from default activator Application

- Removal of all artifacts of activator and SBT
- Remove the ApplicationTimer as it caused an exception because the ApplicationLifecycle could not be injected.
