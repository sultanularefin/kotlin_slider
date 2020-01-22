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



1.https://developer.android.com/studio/releases/gradle-plugin → Gradle update → done form 4.4.1 to 5.4.1
2. https://developer.android.com/jetpack/androidx/migrate


