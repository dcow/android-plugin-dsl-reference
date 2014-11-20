# Android Gradle Plugin Docs

https://dcow.github.io/android-plugin-dsl-reference

Documentation for the Android Gradle plugin. I generated them from the
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

You can [view them on gh-pages](https://dcow.github.io/android-gradle-plugin-docs).
