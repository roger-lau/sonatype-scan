# Sonatype Nexus Lifecycle Scanning

### CLI Scanning for .Net Framework project in Windows machine
```
Requirement:
1. Must use Nuget as package manager in the project
2. Have Java JDK 1.8 installed
```
1. [Download this git repository](https://github.com/roger-lau/sonatype-scan/archive/master.zip)
2. Copy the `packages.config` or `.csproj` of your project into this folder
3. Run `nuget restore packages.config -OutputDirectory packages`
4. A new folder `packages` is created with all of the downloaded packages
5. Run `java -jar ../nexus-iq-cli.jar -i [application id] -s [server URL] -a [username:password] packages`

```
Refer to email for [application id]
```
