[![](https://travis-ci.org/imagej/imagej-command-archetype.svg?branch=master)](https://travis-ci.org/imagej/imagej-command-archetype)

imagej-command-archetype
========================

Maven archetype based on [https://github.com/imagej/example-imagej-command](https://github.com/imagej/example-imagej-command).

Usage
-----

1. `mvn install` this repository

2. Subsequently, you can start the interactive creation mode that let's you select a GAV for a new `Command` that will be created in a new subdirectory of the current directory with the name of your `Command`'s `artifactId`:

```
$ mvn org.apache.maven.plugins:maven-archetype-plugin:3.0.1:generate \
    -DarchetypeGroupId=net.imagej \
    -DarchetypeArtifactId=imagej-command-archetype \
    -DarchetypeVersion=0.0.1-SNAPSHOT
```

**Interactive mode for GAV definition:**
```
[INFO] Scanning for projects...
[INFO]                                                                         
[INFO] ------------------------------------------------------------------------
[INFO] Building Maven Stub Project (No POM) 1
[INFO] ------------------------------------------------------------------------
[INFO] 
[INFO] >>> maven-archetype-plugin:3.0.1:generate (default-cli) > generate-sources @ standalone-pom >>>
[INFO] 
[INFO] <<< maven-archetype-plugin:3.0.1:generate (default-cli) < generate-sources @ standalone-pom <<<
[INFO] 
[INFO] --- maven-archetype-plugin:3.0.1:generate (default-cli) @ standalone-pom ---
[INFO] Generating project in Interactive mode
[INFO] Archetype repository not defined. Using the one from [net.imagej:imagej-command-archetype:0.0.1-SNAPSHOT] found in catalog local
Define value for property 'groupId': com.mycompany
Define value for property 'artifactId': MyCommand
Define value for property 'version' 1.0-SNAPSHOT: : 0.1.0-SNAPSHOT
Define value for property 'package' com.mycompany: : 
Define value for property 'description': My awesome description
Define value for property 'developerId' stefan: : stelfrich
Define value for property 'developerName': Stefan
Define value for property 'developerUrl' https://imagej.net/User:stelfrich: : 
Define value for property 'inceptionYear' 2017: : 
Define value for property 'main-class' com.mycompany.MyCommand: : 
Define value for property 'name': My awesome command
Define value for property 'organizationId': imagej
Define value for property 'organizationName': ImageJ
Define value for property 'organizationUrl' https://github.com/imagej: : 
Define value for property 'scmConnection' scm:git:git://github.com/imagej/MyCommand: : 
Define value for property 'scmDeveloperConnection' scm:git:git@github.com:imagej/MyCommand: : 
Define value for property 'scmUrl' https://github.com/imagej/MyCommand: : 
Define value for property 'url' https://imagej.net/MyCommand: : 
Define value for property 'urlIssueManagement' https://github.com/imagej/MyCommand/issues: : 
Confirm properties configuration:
groupId: com.mycompany
artifactId: MyCommand
version: 0.1.0-SNAPSHOT
package: com.mycompany
description: My awesome description
developerId: stelfrich
developerName: Stefan
developerUrl: https://imagej.net/User:stelfrich
inceptionYear: 2017
main-class: com.mycompany.MyCommand
name: My awesome command
organizationId: imagej
organizationName: ImageJ
organizationUrl: https://github.com/imagej
scmConnection: scm:git:git://github.com/imagej/MyCommand
scmDeveloperConnection: scm:git:git@github.com:imagej/MyCommand
scmUrl: https://github.com/imagej/MyCommand
url: https://imagej.net/MyCommand
urlIssueManagement: https://github.com/imagej/MyCommand/issues
 Y: :
```
