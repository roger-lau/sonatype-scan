# Sonatype Nexus Lifecycle Scanning

## .Net Framework
### Using CLI in Windows machine
```
Requirement:
1. Must use Nuget as package manager in the project
2. Have Java JDK 1.8 installed
```
1. Copy `packages.config` to a new folder
2. Download [nuget.exe](nuget.exe)
3. Copy nuget.exe to the folder
3. In command line, navigate to the folder and run `nuget restore packages.config -OutputDirectory packages`
4. Download [Nexus IQ CLI jar file](/nexus-iq-cli.jar)
5. Run `java -jar nexus-iq-cli.jar -i [application id] -s [server URL] -a [username:password] packages`