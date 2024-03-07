<!-- BEGIN_TF_DOCS -->
## Documentation


### Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.14 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >= 2.0.0 |

### Modules

No modules.

### Resources

| Name | Type |
|------|------|
| [aws_secretsmanager_secret.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/secretsmanager_secret) | resource |
| [aws_secretsmanager_secret_version.this](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/secretsmanager_secret_version) | resource |

### Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_description"></a> [description](#input\_description) | Description  of secret. | `string` | `""` | no |
| <a name="input_kms_key_id"></a> [kms\_key\_id](#input\_kms\_key\_id) | KMS Key ID to encrypt the secret. KMS key arn or alias can be used. | `string` | `""` | no |
| <a name="input_name"></a> [name](#input\_name) | Name of secret to store. | `string` | n/a | yes |
| <a name="input_policy"></a> [policy](#input\_policy) | Resource IAM policy which controls access to the secret. | `string` | `""` | no |
| <a name="input_tags"></a> [tags](#input\_tags) | Resource tags. | `map(string)` | `{}` | no |
| <a name="input_value"></a> [value](#input\_value) | Secret value to store. | `string` | `""` | no |
| <a name="input_values"></a> [values](#input\_values) | Secrets maps to store. | `map(string)` | `{}` | no |

### Outputs

| Name | Description |
|------|-------------|
| <a name="output_arn"></a> [arn](#output\_arn) | AWS Secret Manager secret ARN |
| <a name="output_id"></a> [id](#output\_id) | AWS Secret Manager secret ID |

<!-- END_TF_DOCS -->
