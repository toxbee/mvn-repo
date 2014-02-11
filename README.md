## What?

__mvn-repo__ is a central maven repository for anyone to use.

## How to use

Simply add the repository to your build.gradle file:
```groovy
repositories {
	maven {
		url 'https://github.com/toxbee/mvn-repo/raw/master/maven-deploy'
	}
	mavenCentral()
}
```

And you can use the artifacts like this:
```groovy
dependencies {
	compile 'net.simonvt.numberpicker:android-numberpicker:1.0.0'
	compile 'org.osmdroid:bonuspack:4.0.0-SNAPSHOT'

	// fimpl: https://github.com/toxbee/fimpl
	compile 'se.toxbee.fimpl:fimpl-annotate:0.1.1'
	compile 'se.toxbee.fimpl:fimpl-api:0.1.1'
	compile 'se.toxbee.fimpl:fimpl-common:0.1.1'
	compile 'se.toxbee.fimpl:fimpl-metainf:0.1.1'
}
```

Optionally you can add these gradle plugins to the buildscripts:
```groovy
buildscript {
	repositories {
		maven {
			url 'https://github.com/toxbee/mvn-repo/raw/master/maven-deploy'
		}
		mavenCentral()
	}
	dependencies {
		classpath 'se.toxbee.lgio:gradle-plugin-lgio:0.1'
	}
}
```

## License:
The licenses are provided by the individual libary owner.

This "mvn-repo" utilizes these libaries and won´t provide any support, responsibility or licenses itself.
