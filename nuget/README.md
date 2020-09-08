# Sonatype Nexus Lifecycle - .Net Framework project

### Download .Net Framework project dependencies


```
Requirement:
1. Must use Nuget as package manager in the project
2. Have Java JDK 1.8 installed (for CLI scan only)
```
1. [Download this git repository](https://github.com/roger-lau/sonatype-scan/archive/master.zip)
2. Copy the `packages.config` or `.csproj` of your project into this folder
3. Run `nuget restore packages.config -OutputDirectory packages`
4. A new folder `packages` is created with all of the downloaded packages

### Perform the scan
##### Method 1
5. Compress `packages` folder as a zip and scan from the UI or run `java -jar ../nexus-iq-cli.jar -i [application id] -s [server URL] -a [username:password] packages`
