# Sonatype Nexus Lifecycle Scanning

### CLI Scanning for iOS Cocoapods project
```
Requirement:
1. Must have Java JDK 1.8 installed
```
1. [Download this git repository](https://github.com/roger-lau/sonatype-scan/archive/master.zip)
2. Copy the `Podfile.lock` of your project into this folder. Replace the sample file.
5. Run `java -jar ../nexus-iq-cli.jar -i [application id] -s [server URL] -a [username:password] Podfile.lock`

```
Refer to email for [application id]
```