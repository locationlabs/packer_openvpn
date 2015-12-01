## Overview

This repository contains configurations for using Packer to build an AWS AMI that define
a box that can be used as an OpenVPN server.

## Source Image
This image is based on the [docker-base][] image. You can find the AMI id of that image
in Atlas.

## Release Process

Once your changes are merged to master you need to get the definitions
built by [Atlas][]. You only need to push to master to kick off a build in Atlas.

### Instance-store definitions

## Artifacts

Once Atlas is done building you can find the latest images here:

* [AWS AMIs][]

For an AMI, you can find it's id by looking at the metadata in Atlas.

[docker-base]: https://github.com/locationlabs/packer_docker-base
[Atlas]: https://atlas.hashicorp.com
[AWS AMIs]: https://atlas.hashicorp.com/llabs/artifacts/openvpn/types/amazon.ami
