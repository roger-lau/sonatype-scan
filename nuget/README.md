# Sonatype Nexus Lifecycle — .Net Framework Project in Windows

### Download .Net Framework project packages
```
Requirement:
1. Must use Nuget as package manager in the project
2. Must have Java JDK 1.8 installed (for CLI scan only)
```
1. [Download this git repository](https://github.com/roger-lau/sonatype-scan/archive/master.zip)
2. Copy the `packages.config` or `.csproj` of your project into this folder
3. In CLI, run `nuget.exe restore [packages.config | filename.csproj] -OutputDirectory packages`
4. A new folder `packages` is created with all of the downloaded packages


### Perform the scan

#### Method 1: CLI
1. Run `java -jar ../nexus-iq-cli.jar -i [application id] -s [server URL] -a [username:password] .`
2. Open the report link to view the report


##### Method 2: Upload from UI
1. Compress `packages` folder as a zip
2. In Nexus IQ Server, navigate to `Orgs & Policies`
3. Choose the application from the left navigation menu
4. Navigate to `Actions` dropdown list and choose `Evaluate Binary`
5. Upload the zip file


