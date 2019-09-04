# multi-org-config-template

This is a template for creating new multi-org configuration repositories. To create a new multi-org repository, please follow the steps outlined [here](https://help.github.com/en/articles/creating-a-repository-from-a-template).

## Getting Started

Configuration values are specified in a `config.json` file.
This file must exist in the root directory.
The default file provided in this repository has the minimal required configuration needed to get started.
Some configuration values are optional, and do not need to be specified.
In this case, the configuration value will be defaulted to the one defined by the parent organization.

Below is a sample of the `config.json` file.

```json
{
  "parentId": "nextgen",
  "host": "nextgen-suborg"
}
```

## Options

The following options are valid.

Option|Type|Required|Description
---|---|---|---
parentId|String|Yes|The parent id for the sub-org.
host|String|Yes|The host name for the sub-org. This value will be used to construct the public facing url in the format `host.jemstep.com`.
