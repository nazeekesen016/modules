## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | 4.54.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_eip.fornat](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) | resource |
| [aws_internet_gateway.gw](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/internet_gateway) | resource |
| [aws_nat_gateway.forprivatesubnets](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway) | resource |
| [aws_route_table.private_subnets](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table.rt](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table_association.a](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.private_routes](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_subnet.private-subnets](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.subnet1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_vpc.my-vpc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc) | resource |
| [aws_availability_zones.available](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/availability_zones) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_env"></a> [env](#input\_env) | Name of Environment | `string` | `""` | no |
| <a name="input_name"></a> [name](#input\_name) | Name of Virtual Private Cloud | `string` | `""` | no |
| <a name="input_namesg"></a> [namesg](#input\_namesg) | Name of Security Group | `string` | `"terraform"` | no |
| <a name="input_private-subnet-id"></a> [private-subnet-id](#input\_private-subnet-id) | Identification of subnet | `list` | `[]` | no |
| <a name="input_private-subnet-name"></a> [private-subnet-name](#input\_private-subnet-name) | Provides an VPC subnet resource. | `map` | `{}` | no |
| <a name="input_private-subnets-cidr-block"></a> [private-subnets-cidr-block](#input\_private-subnets-cidr-block) | n/a | `list` | <pre>[<br>  "10.5.4.0/24",<br>  "10.5.5.0/24",<br>  "10.5.6.0/24"<br>]</pre> | no |
| <a name="input_subnet-id"></a> [subnet-id](#input\_subnet-id) | Identification of subnet | `list(string)` | `[]` | no |
| <a name="input_subnet-name"></a> [subnet-name](#input\_subnet-name) | value | `string` | `"Provides an VPC subnet resource."` | no |
| <a name="input_subnet_id"></a> [subnet\_id](#input\_subnet\_id) | Identification of subnet | `list(string)` | `[]` | no |
| <a name="input_subnets-cidr-block"></a> [subnets-cidr-block](#input\_subnets-cidr-block) | n/a | `list` | <pre>[<br>  "10.5.1.0/24",<br>  "10.5.2.0/24",<br>  "10.5.3.0/24"<br>]</pre> | no |
| <a name="input_vpc-cidr-block"></a> [vpc-cidr-block](#input\_vpc-cidr-block) | Range for the subnet, in CIDR notation | `string` | `"10.5.0.0/16"` | no |
| <a name="input_vpc_id"></a> [vpc\_id](#input\_vpc\_id) | Identification of VPC | `string` | `""` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_private-subnet-id"></a> [private-subnet-id](#output\_private-subnet-id) | Identification of private subnet |
| <a name="output_public_subnet_ids"></a> [public\_subnet\_ids](#output\_public\_subnet\_ids) | Identification of subnet |
| <a name="output_vpc_id"></a> [vpc\_id](#output\_vpc\_id) | Identification of VPC |
