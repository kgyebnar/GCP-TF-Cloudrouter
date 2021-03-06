### subnetwork - Network Google Cloud Platform 

Manages a subnetwork within GCE.

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| name | Network name to create on GCP | string | - | yes |
| vpc | Name of the VPC you want to create the subnet in | string | - | yes |
| subnetwork-region | The region this subnetwork will be created in. If unspecified, this defaults to the region configured in the provider. | string | - | no |
| ip_cidr_range |  The IP address range that machines in this network are assigned to | string | - | yes |

## Outputs

| Name | Description |
|------|-------------|
| gateway_address | The IP address of the gateway |
| self_link | The URL of the created resource |

## Docs 

- module docs: https://github.com/tasdikrahman/terraform-gcp-network-subnet/blob/master/README.md
- https://www.terraform.io/docs/providers/google/r/compute_subnetwork.html
- https://cloud.google.com/compute/docs/vpc/#vpc_networks_and_subnets