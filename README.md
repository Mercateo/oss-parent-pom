
### Parent POM for Open-Source Projects published by Mercateo AG

This POM provides some reasonable default plugin configurations. In order to disable preconfigured plugins, add a .noXXXX File to the root of your repository. (See pom.xml for exact filenames)

To use this in Mercateo-OSS projects define a parent in your ```pom.xml```

```
<parent>
	<groupId>com.mercateo.oss</groupId>
	<artifactId>oss-parent-pom</artifactId>
	<version>1.0.1</version> <!-- or the current version -->
</parent>
```
---

#### Changelog:

1.0.2: 
* updated owasp dependency to 3.3.0

1.0.1: 
* owasp plugin now skips scanning provided/runtime/test/system-scoped artifacts

1.0.0:	
* groupId has changed from ```com.mercateo.oss.parent``` to ```com.mercateo.oss```
* owasp plugin dependency upgraded to 3.2.1

