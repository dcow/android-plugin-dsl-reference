# Android Gradle Plugin Docs

The tools team has finally published an official version of the documentation. I will no longer be updating this repository. The official docs are located at

http://google.github.io/android-gradle-dsl/current

For reference purposes, below you can find steps to build the docs yourself (with links updated to the official docs).

Documentation for the Android Gradle plugin. I generated it from the
[android sdk project sources](http://tools.android.com/build).

## OSX

    $ cd path/to/sdk-repo

(e.g. `studio-master-dev` or `gradle_0.14.4`)

    $ repo sync
    $ cd tools
    $ chmod u+w gradle.properties
    $ echo "org.gradle.java.home=$(/usr/libexec/java_home -v 1.6)" >> gradle.properties
    $ ./gradlew docsAll

Docs live in:

    out/build/base/docs/build/docs/dsl

You can [view them on gh-pages](http://google.github.io/android-gradle-dsl/current)
