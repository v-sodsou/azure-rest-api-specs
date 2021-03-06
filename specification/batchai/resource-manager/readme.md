# Batch AI SDK

> see https://aka.ms/autorest

This is the AutoRest configuration file for Batch AI SDK.

---
## Getting Started
To build the SDK for Batch AI, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration



### Basic Information
These are the global settings for the Batch AI.

``` yaml
openapi-type: arm
tag: package-2017-09-preview
```


### Tag: package-2017-09-preview

These settings apply only when `--tag=package-2017-09-preview` is specified on the command line.

``` yaml $(tag) == 'package-2017-09-preview'
input-file: 
- Microsoft.BatchAI/2017-09-01-preview/BatchAI.json
```

---
# Code Generation


## CSharp Settings

These settings apply only when `--csharp` is specified on the command line.
Please also specify `--csharp-sdks-folder=<path to "SDKs" directory of your azure-sdk-for-net clone>`.

``` yaml $(csharp)
csharp:
  azure-arm: true
  license-header: MICROSOFT_MIT_NO_VERSION
  namespace: Microsoft.Azure.Management.BatchAI
  payload-flattening-threshold: 1
  output-folder: $(csharp-sdks-folder)/BatchAI/Management.BatchAI/Generated
  clear-output-folder: true
```