greadle update →

https://developer.android.com/studio/releases/gradle-plugin

buildscript {
    repositories {
        // Gradle 4.1 and higher include support for Google's Maven repo using
        // the google() method. And you need to include this repo to download
        // Android Gradle plugin 3.0.0 or higher.
        google()
        ...
    }
    dependencies {
        classpath 'com.android.tools.build:gradle:3.5.2'
    }
}





let us migrate to android x-→



1. https://developer.android.com/studio/releases/gradle-plugin → Gradle update → done form 4.4.1 to 5.4.1
2. https://developer.android.com/jetpack/androidx/migrate



3. update success:

```json
taxi@taxi-HP-ProBook-4540s:~/Downloads/Kotlin_Image_Slider$ ./gradlew clean
Starting a Gradle Daemon, 4 stopped Daemons could not be reused, use --status for details

> Configure project :app
WARNING: Configuration 'compile' is obsolete and has been replaced with 'implementation' and 'api'.
It will be removed soon. For more information see: http://d.android.com/r/tools/update-dependency-configurations.html

BUILD SUCCESSFUL in 55s
2 actionable tasks: 2 executed
taxi@taxi-HP-ProBook-4540s:~/Downloads/Kotlin_Image_Slider$

```

4. https://stackoverflow.com/questions/53448450/how-to-resolve-error-failed-to-resolve-org-jetbrains-kotlinkotlin-stdlib-jre7/53448758

```json

These are the new valid dependencies as of Kotlin 1.3.0:

implementation "org.jetbrains.kotlin:kotlin-stdlib-jdk7:$kotlin_version"
implementation "org.jetbrains.kotlin:kotlin-stdlib-jdk8:$kotlin_version"
Where $kotlinVersion is either a variable containing the version, or a hard-coded version (i.e. 1.3.0)
```
5. https://kotlinlang.org/docs/reference/using-gradle.html

