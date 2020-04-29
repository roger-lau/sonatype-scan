# Sonatype Nexus Lifecycle Scanning

## .Net Framework
### Command Line Interface
```
Requirement: Must use Nuget as package manager in the project
```
1. Copy `packages.config` to a new folder
2. Download [nuget.exe](https://docs.microsoft.com/en-us/nuget/install-nuget-client-tools)
3. Copy nuget.exe to the folder
3. In command line, navigate to the folder and run `nuget restore packages.config -OutputDirectory packages`
4. Download cli.jar