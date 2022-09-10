# DropwizardExample

Creation Process
---

```
C:\Projects> mvn archetype:generate -DarchetypeGroupId=io.dropwizard.archetypes -DarchetypeArtifactId=java-simple -DarchetypeVersion=2.1.1

[INFO] Scanning for projects...
[INFO]
[INFO] ------------------< org.apache.maven:standalone-pom >-------------------
[INFO] Building Maven Stub Project (No POM) 1
[INFO] --------------------------------[ pom ]---------------------------------
[INFO]
[INFO] >>> maven-archetype-plugin:3.2.0:generate (default-cli) > generate-sources @ standalone-pom >>>
[INFO]
[INFO] <<< maven-archetype-plugin:3.2.0:generate (default-cli) < generate-sources @ standalone-pom <<<
[INFO]
[INFO]
[INFO] --- maven-archetype-plugin:3.2.0:generate (default-cli) @ standalone-pom ---
[INFO] Generating project in Interactive mode
[INFO] Archetype repository not defined. Using the one from [io.dropwizard.archetypes:java-simple:4.0.0-beta.2] found in catalog remote
Downloading from central: https://repo.maven.apache.org/maven2/io/dropwizard/archetypes/java-simple/2.1.1/java-simple-2.1.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/io/dropwizard/archetypes/java-simple/2.1.1/java-simple-2.1.1.pom (1.5 kB at 4.4 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/io/dropwizard/archetypes/dropwizard-archetypes/2.1.1/dropwizard-archetypes-2.1.1.pom
Downloaded from central: https://repo.maven.apache.org/maven2/io/dropwizard/archetypes/dropwizard-archetypes/2.1.1/dropwizard-archetypes-2.1.1.pom (8.1 kB at 24 kB/s)
Downloading from central: https://repo.maven.apache.org/maven2/io/dropwizard/archetypes/java-simple/2.1.1/java-simple-2.1.1.jar
Downloaded from central: https://repo.maven.apache.org/maven2/io/dropwizard/archetypes/java-simple/2.1.1/java-simple-2.1.1.jar (6.2 kB at 15 kB/s)
Define value for property 'groupId': local.snk
Define value for property 'artifactId': dropwizardExample
Define value for property 'version' 1.0-SNAPSHOT: :
Define value for property 'package' local.snk: :
[INFO] Using property: description = null
Define value for property 'name': DropwizardExample
[INFO] Using property: shaded = true
Confirm properties configuration:
groupId: local.snk
artifactId: dropwizardExample
version: 1.0-SNAPSHOT
package: local.snk
description: null
name: DropwizardExample
shaded: true
Y: :
[INFO] ----------------------------------------------------------------------------
[INFO] Using following parameters for creating project from Archetype: java-simple:2.1.1
[INFO] ----------------------------------------------------------------------------
[INFO] Parameter: groupId, Value: local.snk
[INFO] Parameter: artifactId, Value: dropwizardExample
[INFO] Parameter: version, Value: 1.0-SNAPSHOT
[INFO] Parameter: package, Value: local.snk
[INFO] Parameter: packageInPathFormat, Value: local/snk
[INFO] Parameter: package, Value: local.snk
[INFO] Parameter: version, Value: 1.0-SNAPSHOT
[INFO] Parameter: name, Value: DropwizardExample
[INFO] Parameter: groupId, Value: local.snk
[INFO] Parameter: description, Value: null
[INFO] Parameter: shaded, Value: true
[INFO] Parameter: artifactId, Value: dropwizardExample
[INFO] Project created from Archetype in dir: C:\Projects\dropwizardExample
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  01:44 min
[INFO] Finished at: 2022-09-10T13:03:58+05:30
[INFO] ------------------------------------------------------------------------

```

How to start the DropwizardExample application
---

1. Run `mvn clean install` to build your application
1. Start application with `java -jar target/dropwizardExample-1.0-SNAPSHOT.jar server config.yml`
1. To check that your application is running enter url `http://localhost:8080`

Health Check
---

To see your applications health enter url `http://localhost:8081/healthcheck`
