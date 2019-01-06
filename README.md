
### Parent POM for Open-Source Projects published by Mercateo AG

This POM provides some reasonable default plugin configurations. In order to disable preconfigured plugins, add a .noXXXX File to the root of your repository. (See pom.xml for exact filenames)

To use this in Mercateo-OSS projects define a parent in your ```pom.xml```

```
<parent>
	<groupId>com.mercateo.oss</groupId>
	<artifactId>oss-parent-pom</artifactId>
	<version>1.0.3</version> <!-- or the current version -->
</parent>
```
---

#### Changelog:

1.0.7: 
* added -Dossrh to release plugin configuration

1.0.6:
* added src/* to license plugin, so that tests also contain a license header

1.0.5:
* added impsort plugin to sort imports regardless of IDE configuration
* configured license plugin to use /* instead of javadoc style comments for java & kotlin

1.0.3:
* updated JaCoCo dependency to 0.8.2
* make maven release plugin usable

1.0.2: 
* updated owasp dependency to 3.3.0

1.0.1: 
* owasp plugin now skips scanning provided/runtime/test/system-scoped artifacts

1.0.0:	
* groupId has changed from ```com.mercateo.oss.parent``` to ```com.mercateo.oss```
* owasp plugin dependency upgraded to 3.2.1

---

#### Release

perform the following commands:

```
mvn release:prepare
mvn release:perform -Poss.release-sign-artifacts
```
