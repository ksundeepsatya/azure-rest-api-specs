# TimeSeriesInsights
    
> see https://aka.ms/autorest

This is the AutoRest configuration file for TimeSeriesInsights.



---
## Getting Started 
To build the SDK for TimeSeriesInsights, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration



### Basic Information 
These are the global settings for the TimeSeriesInsights API.

``` yaml
openapi-type: arm
tag: package-2017-11-15
```


### Tag: package-2017-02-preview

These settings apply only when `--tag=package-2017-02-preview` is specified on the command line.

``` yaml $(tag) == 'package-2017-02-preview'
input-file:
- Microsoft.TimeSeriesInsights/preview/2017-02-28-preview/timeseriesinsights.json
```

### Tag: package-2017-11-15

These settings apply only when `--tag=package-2017-11-15` is specified on the command line.

``` yaml $(tag) == 'package-2017-11-15'
input-file:
- Microsoft.TimeSeriesInsights/stable/2017-11-15/timeseriesinsights.json
```

## Go

These settings apply only when `--go` is specified on the command line.

``` yaml $(go)
go:
  license-header: MICROSOFT_APACHE_NO_VERSION
  clear-output-folder: true
  namespace: timeseriesinsights
```

### Tag: package-2017-11-15 and go

These settings apply only when `--tag=package-2017-11-15 --go` is specified on the command line.
Please also specify `--go-sdk-folder=<path to the root directory of your azure-sdk-for-go clone>`.

``` yaml $(tag)=='package-2017-11-15' && $(go)
output-folder: $(go-sdk-folder)/services/timeseriesinsights/mgmt/2017-11-15/timeseriesinsights
```
