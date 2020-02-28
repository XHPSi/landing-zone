# landing-zone

Vendored copy of the AWS LandingZone solution using CloudFormation.

This repository contains the AWS LandingZone solution from version 1.0.2 until 2.3.1

## repository structure

The repository contains 2 directories, `unzip` and `zip`.

### zip

The `zip` directory contains the zip-files for the respective landing-zone-version. You can use the zip-files directly and unzip them in a place to work on them.

### unzip

The `unzip` directory contains the up-to-date landingzone files extracted from the zip-file of the respective landing-zone-version. Depending on the git-commit of this repositry/git tag, the `unzip` directorie's file-content changes. This way it is possible to track what are the actual file-changes between each landing-zone.

## download zip-files

You can download the zip-files yourself using the `downloadLandingZones.sh` shell-script. The script downloads all resources, including those who had typos.

## Warnings

Be aware that setting up a Landing Zone is no trivial task. AWS recommends that AWS ProServe or an AWS Partner setup Landing Zones. That said, it is possible to setup and manage a Landing Zone yourself if you're up for a lot of heavy reading, understanding, and troubleshooting. These are the four sources of truth for Landing Zone that do not expire. They are updated regularly, so setup a URL monitor to make sure you're working off of the latest versions.

http://www.awslandingzone.com/guides/aws-landing-zone-implementation-guide.pdf
http://www.awslandingzone.com/guides/aws-landing-zone-developer-guide.pdf
http://www.awslandingzone.com/guides/aws-landing-zone-user-guide.pdf
http://www.awslandingzone.com/guides/aws-landing-zone-upgrade-guide.pdf

The better route for most folks is to use Control Tower to manage your Landing Zone.

https://aws.amazon.com/controltower/
