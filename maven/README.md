# Sonatype Nexus Lifecycle — Maven Project

### Download Maven project packages
```
Requirement:
1. Must use Maven as package manager in the project
2. Must have Maven build tool installed
3. Must have Java JDK 1.8 installed (for CLI only)
```
1. [Download this git repository](https://github.com/roger-lau/sonatype-scan/archive/master.zip)
2. Copy the `pom.xml` of your project into this folder
3. Run `mvn install`
5. Run `java -jar ../nexus-iq-cli.jar -i [application id] -s [server URL] -a [username:password] .`


### Perform the scan

#### Method 1: CLI
1. Run this command
`java -jar ../nexus-iq-cli.jar -i [application id] -s [server URL] -a [username:password] .`

2. Open the report link to view the report


##### Method 2: Upload from UI
1. Compress this folder as a zip
2. In Nexus IQ Server, navigate to `Orgs & Policies`
3. Choose the application from the left navigation menu
4. Navigate to `Actions` dropdown list and choose `Evaluate Binary`
5. Upload the zip file
