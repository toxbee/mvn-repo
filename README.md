How to use
========

Simply add the repository to your build.gradle file:

    repositories {
        maven {
            url 'https://github.com/Centril/mvn-repo/raw/master/maven-deploy'
        }
        mavenCentral()
    }

And you can use the artifacts like this:

    dependencies {
        compile 'net.simonvt.numberpicker:android-numberpicker:1.0.0'
    }

License:
--------
The licenses are provided by the individual libary owner.

This "mvn-repo" utilizes these libaries and won´t provide any support, responsibility or licenses itself.
