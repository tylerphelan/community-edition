# calico Package

This package provides networking and network security solution for containers using [calico](https://www.projectcalico.org/).

## Components

## Configuration

The following configuration values can be set to customize the calico installation.

### Global

| Value | Required/Optional | Description |
|-------|-------------------|-------------|
| `infraProvider` | Required | The infrastructure provider in use. One of: `aws`, `azure`, `vsphere`, `docker`. |
| `ipFamily` | Optional | The IP family calico should be configured with. Defaults to `ipv4`. One of: `ipv4`, `ipv6`, `ipv4,ipv6` (IPv4-primary dualstack), or `ipv6,ipv4` (IPv6-primary dualstack) |

### calico Configuration

| Value | Required/Optional | Description |
|-------|-------------------|-------------|
| `calico.config.clusterCIDR` | Optional | The pod network CIDR. Default value is empty because it can be auto detected. |
| `calico.config.vethMTU` | Optional | MTU size. Default is `0`, which means it will be auto detected. |

## Usage Example

To learn more about how to use calico refer to [calico documentation](https://docs.projectcalico.org/about/about-calico)
