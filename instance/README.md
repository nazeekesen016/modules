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
| [aws_instance.BASTION](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance) | resource |
| [aws_security_group.only_ssh_bositon](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |
| [aws_ami.ubuntu](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_bastion-host-name"></a> [bastion-host-name](#input\_bastion-host-name) | value | `string` | `""` | no |
| <a name="input_env"></a> [env](#input\_env) | value | `string` | `""` | no |
| <a name="input_instance-type"></a> [instance-type](#input\_instance-type) | value | `string` | `""` | no |
| <a name="input_name-sg"></a> [name-sg](#input\_name-sg) | value | `string` | `""` | no |
| <a name="input_subnet_id"></a> [subnet\_id](#input\_subnet\_id) | n/a | `list(string)` | `[]` | no |
| <a name="input_vpc-id"></a> [vpc-id](#input\_vpc-id) | n/a | `any` | n/a | yes |

## Outputs

No outputs.
