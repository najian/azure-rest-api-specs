# SecurityAndCompliance

> see https://aka.ms/autorest

This is the AutoRest configuration file for SecurityAndCompliance.



---
## Getting Started
To build the SDK for SecurityAndCompliance, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration



### Basic Information
These are the global settings for the SecurityAndCompliance API.

``` yaml
title: SecurityAndComplianceClient
description: Security And Compliance Client
openapi-type: arm
tag: package-2021-03-08
```

### Tag: package-2021-01-11

These settings apply only when `--tag=package-2021-01-11` is specified on the command line.

``` yaml $(tag) == 'package-2021-01-11'
input-file:
- Microsoft.SecurityAndCompliance/stable/2021-01-11/common-types.json
- Microsoft.SecurityAndCompliance/stable/2021-01-11/privateLinkServicesForEDMUpload.json
- Microsoft.SecurityAndCompliance/stable/2021-01-11/privateLinkServicesForM365ComplianceCenter.json
- Microsoft.SecurityAndCompliance/stable/2021-01-11/privateLinkServicesForM365SecurityCenter.json
- Microsoft.SecurityAndCompliance/stable/2021-01-11/privateLinkServicesForO365ManagementActivityAPI.json
- Microsoft.SecurityAndCompliance/stable/2021-01-11/privateLinkServicesForSCCPowershell.json
```

### Tag: package-2021-03-08

These settings apply only when `--tag=package-2021-03-08` is specified on the command line.

``` yaml $(tag) == 'package-2021-03-08'
input-file:
- Microsoft.SecurityAndCompliance/stable/2021-03-08/common-types.json
- Microsoft.SecurityAndCompliance/stable/2021-03-08/privateLinkServicesForEDMUpload.json
- Microsoft.SecurityAndCompliance/stable/2021-03-08/privateLinkServicesForM365ComplianceCenter.json
- Microsoft.SecurityAndCompliance/stable/2021-03-08/privateLinkServicesForM365SecurityCenter.json
- Microsoft.SecurityAndCompliance/stable/2021-03-08/privateLinkServicesForO365ManagementActivityAPI.json
- Microsoft.SecurityAndCompliance/stable/2021-03-08/privateLinkServicesForSCCPowershell.json
- Microsoft.SecurityAndCompliance/stable/2021-03-08/privateLinkServicesForMIPPolicySync.json
```

---
# Code Generation


## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by Autorest itself.

``` yaml $(swagger-to-sdk)
swagger-to-sdk:
  - repo: azure-sdk-for-go
  - repo: azure-sdk-for-js
  - repo: azure-sdk-for-node
  - repo: azure-sdk-for-python
  - repo: azure-resource-manager-schemas
```

## Go

See configuration in [readme.go.md](./readme.go.md)

## Java

These settings apply only when `--java` is specified on the command line.
Please also specify `--azure-libraries-for-java-folder=<path to the root directory of your azure-libraries-for-java clone>`.

``` yaml $(java)
azure-arm: true
fluent: true
namespace: com.microsoft.azure.management.securityandcompliance
license-header: MICROSOFT_MIT_NO_CODEGEN
payload-flattening-threshold: 1
output-folder: $(azure-libraries-for-java-folder)/azure-mgmt-securityandcompliance
```

### Java multi-api

``` yaml $(java) && $(multiapi)
batch:
  - tag: package-2021-01-11
```

### Tag: package-2021-01-11 and java

These settings apply only when `--tag=package-2021-01-11 --java` is specified on the command line.
Please also specify `--azure-libraries-for-java=<path to the root directory of your azure-sdk-for-java clone>`.

``` yaml $(tag) == 'package-2021-01-11' && $(java) && $(multiapi)
java:
  namespace: com.microsoft.azure.management.securityandcompliance.v2021_01_11
  output-folder: $(azure-libraries-for-java-folder)/sdk/securityandcompliance/mgmt-v2021_01_11
regenerate-manager: true
generate-interface: true
```

``` yaml $(java) && $(multiapi)
batch:
  - tag: package-2021-03-08
```

### Tag: package-2021-03-08 and java

These settings apply only when `--tag=package-2021-03-08 --java` is specified on the command line.
Please also specify `--azure-libraries-for-java=<path to the root directory of your azure-sdk-for-java clone>`.

``` yaml $(tag) == 'package-2021-03-08' && $(java) && $(multiapi)
java:
  namespace: com.microsoft.azure.management.securityandcompliance.v2021_03_08
  output-folder: $(azure-libraries-for-java-folder)/sdk/securityandcompliance/mgmt-v2021_03_08
regenerate-manager: true
generate-interface: true
```

## Python

See configuration in [readme.python.md](./readme.python.md)





