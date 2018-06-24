
Parent POM for Open-Source Projects published by Mercateo AG

This POM provides some reasonable default plugin configurations. In order to disable preconfigured plugins, add a .noXXXX File to the root of your repository. (See pom.xml for exact filenames)

To use this in Mercateo-OSS projects define a parent in your ```pom.xml```

```
	<parent>
		<groupId>com.mercateo.oss</groupId>
		<artifactId>oss-parent-pom</artifactId>
		<version>1.0.0</version> <!-- or the current version -->
	</parent>

```
---

Changelog:

1.0.0:	
* groupId has changed from ```com.mercateo.oss.parent``` to ```com.mercateo.oss```
* owasp plugin dependency upgraded to 3.2.1

