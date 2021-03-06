# Storage

> see https://aka.ms/autorest

This is the AutoRest configuration file for Storage.



---
## Getting Started
To build the SDK for Storage, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration



### Basic Information
These are the global settings for the Storage API.

``` yaml
openapi-type: arm
tag: package-2019-04
```

### Tag: package-2019-04

These settings apply only when `--tag=package-2019-04` is specified on the command line.

``` yaml $(tag) == 'package-2019-04'
input-file:
- Microsoft.Storage/stable/2019-04-01/storage.json
- Microsoft.Storage/stable/2019-04-01/blob.json

directive:
  - suppress: R3018
    reason: Existing boolean properties
    approved-by: "@fearthecowboy"

  - where:
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/blobServices/default/containers/{containerName}/setLegalHold"].post.operationId
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/blobServices/default/containers/{containerName}/clearLegalHold"].post.operationId
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/regenerateKey"].post.operationId
    suppress: R1003
    reason: APIs return array of values, is not actually a 'list' operation
    approved-by: "@fearthecowboy"

```

### Tag: package-2018-11

These settings apply only when `--tag=package-2018-11` is specified on the command line.

``` yaml $(tag) == 'package-2018-11'
input-file:
- Microsoft.Storage/stable/2018-11-01/storage.json
- Microsoft.Storage/stable/2018-11-01/blob.json

directive:
  - suppress: R3018
    reason: Existing boolean properties
    approved-by: "@fearthecowboy"

  - where:
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/blobServices/default/containers/{containerName}/setLegalHold"].post.operationId
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/blobServices/default/containers/{containerName}/clearLegalHold"].post.operationId
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/regenerateKey"].post.operationId
    suppress: R1003
    reason: APIs return array of values, is not actually a 'list' operation
    approved-by: "@fearthecowboy"

```

### Tag: package-2018-07

These settings apply only when `--tag=package-2018-07` is specified on the command line.

``` yaml $(tag) == 'package-2018-07'
input-file:
- Microsoft.Storage/stable/2018-07-01/storage.json
- Microsoft.Storage/stable/2018-07-01/blob.json
- Microsoft.Storage/preview/2018-03-01-preview/managementpolicy.json

directive:
  - suppress: R3018
    reason: Existing boolean properties
    approved-by: "@fearthecowboy"

  - where:
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/blobServices/default/containers/{containerName}/setLegalHold"].post.operationId
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/blobServices/default/containers/{containerName}/clearLegalHold"].post.operationId
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/regenerateKey"].post.operationId
    suppress: R1003
    reason: APIs return array of values, is not actually a 'list' operation
    approved-by: "@fearthecowboy"

```

### Tag: package-2018-07-only

These settings apply only when `--tag=package-2018-07-only` is specified on the command line.

``` yaml $(tag) == 'package-2018-07-only'
input-file:
- Microsoft.Storage/stable/2018-07-01/storage.json
- Microsoft.Storage/stable/2018-07-01/blob.json
```

### Tag: package-2018-03

These settings apply only when `--tag=package-2018-03` is specified on the command line.

``` yaml $(tag) == 'package-2018-03'
input-file:
- Microsoft.Storage/preview/2018-03-01-preview/storage.json
- Microsoft.Storage/preview/2018-03-01-preview/blob.json

directive:
  - suppress: R3018
    reason: Existing boolean properties
    approved-by: "@fearthecowboy"

  - where:
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/blobServices/default/containers/{containerName}/setLegalHold"].post.operationId
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/blobServices/default/containers/{containerName}/clearLegalHold"].post.operationId
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/regenerateKey"].post.operationId
    suppress: R1003
    reason: APIs return array of values, is not actually a 'list' operation
    approved-by: "@fearthecowboy"

```

### Tag: package-2018-02

These settings apply only when `--tag=package-2018-02` is specified on the command line.

``` yaml $(tag) == 'package-2018-02'
input-file:
- Microsoft.Storage/stable/2018-02-01/storage.json
- Microsoft.Storage/stable/2018-02-01/blob.json

directive:
  - suppress: R3018
    reason: Existing boolean properties
    approved-by: "@fearthecowboy"

  - where:
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/blobServices/default/containers/{containerName}/setLegalHold"].post.operationId
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/blobServices/default/containers/{containerName}/clearLegalHold"].post.operationId
    - $.paths["/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Storage/storageAccounts/{accountName}/regenerateKey"].post.operationId
    suppress: R1003
    reason: APIs return array of values, is not actually a 'list' operation
    approved-by: "@fearthecowboy"

```

### Tag: package-2017-10

These settings apply only when `--tag=package-2017-10` is specified on the command line.

``` yaml $(tag) == 'package-2017-10'
input-file:
- Microsoft.Storage/stable/2017-10-01/storage.json
```

### Tag: package-2017-06

These settings apply only when `--tag=package-2017-06` is specified on the command line.

``` yaml $(tag) == 'package-2017-06'
input-file:
- Microsoft.Storage/stable/2017-06-01/storage.json
```


### Tag: package-2016-12

These settings apply only when `--tag=package-2016-12` is specified on the command line.

``` yaml $(tag) == 'package-2016-12'
input-file:
- Microsoft.Storage/stable/2016-12-01/storage.json
```

### Tag: package-2016-05

These settings apply only when `--tag=package-2016-05` is specified on the command line.

``` yaml $(tag) == 'package-2016-05'
input-file:
- Microsoft.Storage/stable/2016-05-01/storage.json
```

### Tag: package-2016-01

These settings apply only when `--tag=package-2016-01` is specified on the command line.

``` yaml $(tag) == 'package-2016-01'
input-file:
- Microsoft.Storage/stable/2016-01-01/storage.json
```

### Tag: package-2015-06

These settings apply only when `--tag=package-2015-06` is specified on the command line.

``` yaml $(tag) == 'package-2015-06'
input-file:
- Microsoft.Storage/stable/2015-06-15/storage.json
```

### Tag: package-2015-05-preview

These settings apply only when `--tag=package-2015-05-preview` is specified on the command line.

``` yaml $(tag) == 'package-2015-05-preview'
input-file:
- Microsoft.Storage/preview/2015-05-01-preview/storage.json
```


---
# Code Generation


## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by Autorest itself.

``` yaml $(swagger-to-sdk)
swagger-to-sdk:
  - repo: azure-sdk-for-python
    after_scripts:
      - python ./scripts/multiapi_init_gen.py azure-mgmt-storage
  - repo: azure-sdk-for-java
  - repo: azure-sdk-for-go
  - repo: azure-sdk-for-node
  - repo: azure-sdk-for-js
  - repo: azure-sdk-for-ruby
    after_scripts:
      - bundle install && rake arm:regen_all_profiles['azure_mgmt_storage']
```

## Java

These settings apply only when `--java` is specified on the command line.
Please also specify `--azure-libraries-for-java-folder=<path to the root directory of your azure-libraries-for-java clone>`.

``` yaml $(java)
azure-arm: true
fluent: true
namespace: com.microsoft.azure.management.storage
license-header: MICROSOFT_MIT_NO_CODEGEN
payload-flattening-threshold: 2
output-folder: $(azure-libraries-for-java-folder)/azure-mgmt-storage
```

### Java multi-api

``` yaml $(java) && $(multiapi)
batch:
  - tag: package-2018-07
  - tag: package-2018-03
  - tag: package-2018-02
  - tag: package-2017-10
  - tag: package-2016-01
```

### Tag: package-2018-07 and java

These settings apply only when `--tag=package-2018-07 --java` is specified on the command line.
Please also specify `--azure-libraries-for-java-folder=<path to the root directory of your azure-sdk-for-java clone>`.

``` yaml $(tag) == 'package-2018-07' && $(java) && $(multiapi)
java:
  namespace: com.microsoft.azure.management.storage.v2018_07_01
  output-folder: $(azure-libraries-for-java-folder)/storage/resource-manager/v2018_07_01
regenerate-manager: true
generate-interface: true
```

### Tag: package-2018-03 and java

These settings apply only when `--tag=package-2018-03 --java` is specified on the command line.
Please also specify `--azure-libraries-for-java-folder=<path to the root directory of your azure-sdk-for-java clone>`.

``` yaml $(tag) == 'package-2018-03' && $(java) && $(multiapi)
java:
  namespace: com.microsoft.azure.management.storage.v2018_03_01_preview
  output-folder: $(azure-libraries-for-java-folder)/storage/resource-manager/v2018_03_01_preview
regenerate-manager: true
generate-interface: true
```

### Tag: package-2018-02 and java

These settings apply only when `--tag=package-2018-02 --java` is specified on the command line.
Please also specify `--azure-libraries-for-java-folder=<path to the root directory of your azure-sdk-for-java clone>`.

``` yaml $(tag) == 'package-2018-02' && $(java) && $(multiapi)
java:
  namespace: com.microsoft.azure.management.storage.v2018_02_01
  output-folder: $(azure-libraries-for-java-folder)/storage/resource-manager/v2018_02_01
regenerate-manager: true
generate-interface: true
```

### Tag: package-2017-10 and java

These settings apply only when `--tag=package-2017-10 --java` is specified on the command line.
Please also specify `--azure-libraries-for-java-folder=<path to the root directory of your azure-sdk-for-java clone>`.

``` yaml $(tag) == 'package-2017-10' && $(java) && $(multiapi)
java:
  namespace: com.microsoft.azure.management.storage.v2017_10_01
  output-folder: $(azure-libraries-for-java-folder)/storage/resource-manager/v2017_10_01
regenerate-manager: true
generate-interface: true
```

### Tag: package-2016-01 and java

These settings apply only when `--tag=package-2016-01 --java` is specified on the command line.
Please also specify `--azure-libraries-for-java-folder=<path to the root directory of your azure-sdk-for-java clone>`.

``` yaml $(tag) == 'package-2016-01' && $(java) && $(multiapi)
java:
  namespace: com.microsoft.azure.management.storage.v2016_01_01
  output-folder: $(azure-libraries-for-java-folder)/storage/resource-manager/v2016_01_01
regenerate-manager: true
generate-interface: true
```

### Tag: profile-hybrid-2019-03-01

These settings apply only when `--tag=profile-hybrid-2019-03-01` is specified on the command line.
Creating this tag to pick proper resources from the hybrid profile.

``` yaml $(tag) == 'profile-hybrid-2019-03-01'
input-file:
- Microsoft.Storage/stable/2017-10-01/storage.json
```
