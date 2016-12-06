# Build

Q:Can't not build by mvn

```
Failed to execute goal org.apache.maven.plugins:maven-assembly-plugin:2.4:single (make-assembly) on project ManageService: Execution make-assembly of goal org.apache.maven.plugins:maven-assembly-plugin:2.4:single failed: Plugin org.apache.maven.plugins:maven-assembly-plugin:2.4 or one of its dependencies could not be resolved: Failed to collect dependencies at org.apache.maven.plugins:maven-assembly-plugin:jar:2.4 -> org.apache.maven:maven-core:jar:2.2.1 -> org.apache.maven.reporting:maven-reporting-api:jar:2.2.1: Failed to read artifact descriptor for org.apache.maven.reporting:maven-reporting-api:jar:2.2.1: Could not transfer artifact org.apache.maven.reporting:maven-reporting-api:pom:2.2.1 from/to central (http://repo.maven.apache.org/maven2): connect timed out -> [Help 1]

```

A:把build中的170行 <version>2.4</version> 
改成之前的<version>2.2-beta-5</version>

