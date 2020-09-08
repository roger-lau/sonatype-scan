# Sonatype Nexus Lifecycle - PyPi Project


```
Requirement:
1. Must use PyPi as package manager in the project
2. Must have PIP build tool installed
2. Must have Java JDK 1.8 installed (for CLI scan only)
```
### Download PyPi project packages
1. [Download this git repository](https://github.com/roger-lau/sonatype-scan/archive/master.zip)
2. Copy the `requirements.txt` of your project into this folder. Replace the sample file.
3. In CLI, navigate to `packages` folder
3. Run `pip download -r ../requirements.txt`
4. Packages are downloaded into `packages` folder


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


