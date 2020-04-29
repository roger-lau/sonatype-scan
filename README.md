# Sonatype Nexus Lifecycle Scanning

## .Net Framework
### Using CLI in Windows machine
```
Requirement:
1. Must use Nuget as package manager in the project
2. Have Java JDK 1.8 installed
```
1. Download this git repository
2. Copy the `packages.config` of your project in this folder
3. Run `nuget restore packages.config -OutputDirectory packages`
5. Run `java -jar nexus-iq-cli.jar -i [application id] -s [server URL] -a [username:password] packages`