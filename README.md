# cSCM
|  |  |
|--|--|
|Lincense|[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/ctection/cSCM/blob/master/LICENSE)|
|Support |[![Discord](https://img.shields.io/discord/554675435309629451?logo=discord)](https://discord.gg/eaZseHT2F7)|
|Downloads|[![Github all releases](https://img.shields.io/github/downloads/ctection/cSCM/total.svg)](https://GitHub.com/ctection/cSCM/releases/)|
|Build|![GitHub Workflow Status](https://img.shields.io/github/workflow/status/ctection/cSCM/Gradle)|
### Simple Collection Mapping (SCM) Parser

We invented this Data Format to allow advanced Memory Transfers via Networked Sockets.

SCM or Simple Collection Mapping allows us to collect data from multiple HashMaps, lists, Queues, Stacks and other linear or non-linear datatypes and store them in a String. SCM supports multiple Datasets by nature, all included in one String Object.

Here is an example SCM Object during Advanced Handover: ```568511777281933336:3;316980441502449666:568511777281933336;568511777281933336:1;;;```

This is the Basic SCM Syntax Explained:

`:` separates a Key:Value pair. This is essentially one Hashmap or one List entry (2 Column Entry)

`,` indicates the end of a Key:Value pair (EoL Indicator). It essentially indicates a "row" in traditional Database design

`;` acts as a seperator between two Datasets (Each identified by : and ,)

`:`, `,` and `;` can be escaped to not be recognized as operational characters.

Using SCM instead of JSON can result in lower Memory Usage and Data Usage when transferring via Networked Socket, therefore reducing transferring time and allowing for a cleaner Handover.

## Download
|  |  |
|--|--|
|Latest Github Release|[![GitHub release](https://img.shields.io/github/release/ctection/cSCM.svg)](https://GitHub.com/ctection/cSCM/releases/)|
|Maven Central|[![Maven Central](https://img.shields.io/maven-central/v/com.ctection/cSCM?color=gree)](https://search.maven.org/artifact/com.ctection/cSCM/) |
|Commits|![GitHub commits since latest release (by SemVer)](https://img.shields.io/github/commits-since/ctection/cSCM/1.1.0?color=gree&sort=date)|

**Be sure to replace VERSION with the version shown above!**
#### Maven
```XML
<dependencies>
	<dependency>
	  <groupId>com.ctection</groupId>
	  <artifactId>cSCM</artifactId>
	  <version>VERSION</version>
	</dependency>
</dependencies>
```
#### Gradle
```gradle
dependencies {
	implementation 'com.ctection:cSCM:VERSION'
}
```
