# Simple-Sysmon
This is a simple starter configuration for an intro to Atomic Red Team session. It includes basic detections for a few Atomic Red Tests to get you started, and you can improve and build out those detections from there.

## Installation

Download Sysmon from https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon

Extract the files from the downloaded zip file.

Download simple-sysmon.xml from this repo.

When you install Sysmon, it be added as a Windows service using the configuration in a file you specify. Install with the following, from an elevated command prompt:

`sysmon64.exe -i simple-sysmon.xml -accepteula`

## Making Changes

As you make changes to the config file to include new/improved detections, you can load the new configuration with the following:

`sysmon64.exe -c simple-sysmon.xml`
