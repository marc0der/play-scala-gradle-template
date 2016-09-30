# Example Play Java Application Using Gradle

Starting with Gradle 3.1, Play 2.5.x is (partially) supported. 
But there are no examples how to use Play 2.5.x with Gradle 3.1.
This project closes the gap by providing such an example. 

You can simply run it by executing `./gradlew --continous runPlayBinary` on the command line.

## Changes from default activator Application

- Removal of all artifacts of activator and SBT
- Remove the ApplicationTimer as it caused an exception because the ApplicationLifecycle could not be injected.
