# Sonatype Nexus Lifecycle Scanning

### CLI Scanning for Maven project
```
Requirement:
1. Must use Maven as package manager in the project
2. Must have Maven build tool installed
2. Must have Java JDK 1.8 installed
```
1. [Download this git repository](https://github.com/roger-lau/sonatype-scan/archive/master.zip)
2. Copy the `pom.xml` of your project into this folder
3. Run `mvn install`
5. Run `java -jar ../nexus-iq-cli.jar -i [application id] -s [server URL] -a [username:password] .`

```
Refer to email for [application id]
```
