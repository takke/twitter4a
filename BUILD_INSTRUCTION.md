Build Instruction using Gradle
==============================

Guide for Twitter4J Developers / Contributors using Gradle

- makes ```jar```, ```javadoc.jar``` and ```sources.jar```

```bash
$ ./gradlew clean build -x test
```

- mavenLocal : deploys to ```~/.m2/repository/org/twitter4j/```.
```bash
$ ./gradlew publishToMavenLocal
```

- upload to bintray
```bash
$ ./gradlew bintrayUpload
```


Release to Repository
=====================

Modify version name
-------------------

- modify ```versionName```  in ```build.gradle```

Build, upload to bintray
------------------------

```bash
$ ./gradlew clean build -x test
```
```bash
$ ./gradlew bintrayUpload
```
check on bintray
----------------
https://bintray.com/panecraft/maven/Twitter4J

Tagging
-------

```bash
$ git tag -a 4.1.0-beta1 678ee0a
$ git push origin 4.1.0-beta1
```


References
==========

- [まくまく Gradle ノート](http://maku77.github.io/gradle/)
- [Gradle Mavenプラグイン\(Hishidama's Gradle Maven plugin Memo\)](http://www.ne.jp/asahi/hishidama/home/tech/groovy/gradle/maven.html)

- https://github.com/bintray/bintray-examples/blob/master/gradle-example/build.gradle
- https://github.com/bintray/bintray-examples/tree/master/gradle-bintray-plugin-examples
- https://github.com/bintray/gradle-bintray-plugin


TODO
====

- Fix Contributors