# Sonatype Nexus Lifecycle — Cocoapods Project


```
Requirement:
1. Must have Java JDK 1.8 installed
```
### CLI Scanning for iOS Cocoapods project
1. [Download this git repository](https://github.com/roger-lau/sonatype-scan/archive/master.zip)
2. Copy the `Podfile.lock` of your project into this folder. Replace the sample file.
5. Run `java -jar ../nexus-iq-cli.jar -i [application id] -s [server URL] -a [username:password] Podfile.lock`

### References
[Link to Sonatype Guide for Cocoapods application analysis](https://help.sonatype.com/iqserver/analysis/objective-c-application-analysis)