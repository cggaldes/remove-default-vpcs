# remove-default-vpcs
Python script to remove all default VPCs from all regions in AWS.

## Pre-requisite:
```sh
$ pip install botocore boto3
```

## Before running:
Ensure AWS credentials are ready (e.g. ~/.aws/credential).  See Boto [configuring credentials](http://boto3.readthedocs.io/en/latest/guide/configuration.html) 

Quickest way is to use `aws configure` (need AWS CLI installed)

## Usage:
```sh
$ python remove_default_vpcs.py
```

## Options:
```sh
--no-verify-ssl
```
Disable SSL verification.  Could be useful if you are behind proxy.

```sh
--profile=<profile>
```
If you have multiple credential profiles configured.  Boto will use `[default]` profile by default. 

