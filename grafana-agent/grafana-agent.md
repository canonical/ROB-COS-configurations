# Grafana agent
This folder contains configuration examples for the Grafana agent config.

The configurations are river files meant to be used with [flow mode](https://grafana.com/docs/agent/latest/flow/).

## Configurations

- [configuration 1](./configuration-1.river) -- Configuration sharing almost any information available.
- [configuration 2](./configuration-2.river) -- Configuration sharing critical logs, systemd and filesystem only to save bandwith and storage.

You can easilly write your own configuration file with the help of the [Grafana agent configurator](https://grafana.github.io/agent-configurator/).

The resource usage can be estimated following this guide: [Estimate Grafana Agent Flow resource usage](https://grafana.com/docs/agent/latest/flow/tasks/estimate-resource-usage/).
