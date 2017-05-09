# OM PCF Templates

This repository contains JSON templates to deploy and operate [Pivotal Cloud Foundry](https://pivotal.io/platform) with [pivotal-cf/om](https://github.com/pivotal-cf/om).

The templates are suited for product versions listed at the bottom of this README file.

## How to use the templates

Clone this repository and make any necessary adjustments to the JSON template files.
Then, use the `om` CLI tool to PUT the configured JSON files to your OpsManager instance.
Check out the README files in the folders for how to use the `om` tool to achieve a particular task with the JSON templates.

## Templates

- [BOSH Director](./bosh): v1.10.*
- [Pivotal Cloud Foundry](./pcf): v1.10.*
- [JMX Bridge](./products/jmx-bridge): v1.8.*
- [Isolation Segment](./products/isolation-segment): v1.10.*