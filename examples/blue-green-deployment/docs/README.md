# blue-green-deployment

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 1.0 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >= 5.25 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | >= 5.25 |

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_mysql"></a> [mysql](#module\_mysql) | ../../ | n/a |
| <a name="module_mysql_security_group"></a> [mysql\_security\_group](#module\_mysql\_security\_group) | terraform-aws-modules/security-group/aws | ~> 5.0 |
| <a name="module_postgres"></a> [postgres](#module\_postgres) | ../../ | n/a |
| <a name="module_postgres_security_group"></a> [postgres\_security\_group](#module\_postgres\_security\_group) | terraform-aws-modules/security-group/aws | ~> 5.0 |
| <a name="module_vpc"></a> [vpc](#module\_vpc) | terraform-aws-modules/vpc/aws | ~> 5.0 |

## Resources

| Name | Type |
|------|------|
| [aws_availability_zones.available](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/availability_zones) | data source |

## Inputs

No inputs.

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_db_instance_status"></a> [db\_instance\_status](#output\_db\_instance\_status) | The RDS instance status |
| <a name="output_mysql_db_instance_address"></a> [mysql\_db\_instance\_address](#output\_mysql\_db\_instance\_address) | The address of the RDS instance |
| <a name="output_mysql_db_instance_arn"></a> [mysql\_db\_instance\_arn](#output\_mysql\_db\_instance\_arn) | The ARN of the RDS instance |
| <a name="output_mysql_db_instance_availability_zone"></a> [mysql\_db\_instance\_availability\_zone](#output\_mysql\_db\_instance\_availability\_zone) | The availability zone of the RDS instance |
| <a name="output_mysql_db_instance_cloudwatch_log_groups"></a> [mysql\_db\_instance\_cloudwatch\_log\_groups](#output\_mysql\_db\_instance\_cloudwatch\_log\_groups) | Map of CloudWatch log groups created and their attributes |
| <a name="output_mysql_db_instance_endpoint"></a> [mysql\_db\_instance\_endpoint](#output\_mysql\_db\_instance\_endpoint) | The connection endpoint |
| <a name="output_mysql_db_instance_engine"></a> [mysql\_db\_instance\_engine](#output\_mysql\_db\_instance\_engine) | The database engine |
| <a name="output_mysql_db_instance_engine_version_actual"></a> [mysql\_db\_instance\_engine\_version\_actual](#output\_mysql\_db\_instance\_engine\_version\_actual) | The running version of the database |
| <a name="output_mysql_db_instance_hosted_zone_id"></a> [mysql\_db\_instance\_hosted\_zone\_id](#output\_mysql\_db\_instance\_hosted\_zone\_id) | The canonical hosted zone ID of the DB instance (to be used in a Route 53 Alias record) |
| <a name="output_mysql_db_instance_identifier"></a> [mysql\_db\_instance\_identifier](#output\_mysql\_db\_instance\_identifier) | The RDS instance identifier |
| <a name="output_mysql_db_instance_name"></a> [mysql\_db\_instance\_name](#output\_mysql\_db\_instance\_name) | The database name |
| <a name="output_mysql_db_instance_port"></a> [mysql\_db\_instance\_port](#output\_mysql\_db\_instance\_port) | The database port |
| <a name="output_mysql_db_instance_resource_id"></a> [mysql\_db\_instance\_resource\_id](#output\_mysql\_db\_instance\_resource\_id) | The RDS Resource ID of this instance |
| <a name="output_mysql_db_instance_username"></a> [mysql\_db\_instance\_username](#output\_mysql\_db\_instance\_username) | The master username for the database |
| <a name="output_mysql_db_parameter_group_arn"></a> [mysql\_db\_parameter\_group\_arn](#output\_mysql\_db\_parameter\_group\_arn) | The ARN of the db parameter group |
| <a name="output_mysql_db_parameter_group_id"></a> [mysql\_db\_parameter\_group\_id](#output\_mysql\_db\_parameter\_group\_id) | The db parameter group id |
| <a name="output_mysql_db_subnet_group_arn"></a> [mysql\_db\_subnet\_group\_arn](#output\_mysql\_db\_subnet\_group\_arn) | The ARN of the db subnet group |
| <a name="output_mysql_db_subnet_group_id"></a> [mysql\_db\_subnet\_group\_id](#output\_mysql\_db\_subnet\_group\_id) | The db subnet group name |
| <a name="output_postgres_db_instance_address"></a> [postgres\_db\_instance\_address](#output\_postgres\_db\_instance\_address) | The address of the RDS instance |
| <a name="output_postgres_db_instance_arn"></a> [postgres\_db\_instance\_arn](#output\_postgres\_db\_instance\_arn) | The ARN of the RDS instance |
| <a name="output_postgres_db_instance_availability_zone"></a> [postgres\_db\_instance\_availability\_zone](#output\_postgres\_db\_instance\_availability\_zone) | The availability zone of the RDS instance |
| <a name="output_postgres_db_instance_cloudwatch_log_groups"></a> [postgres\_db\_instance\_cloudwatch\_log\_groups](#output\_postgres\_db\_instance\_cloudwatch\_log\_groups) | Map of CloudWatch log groups created and their attributes |
| <a name="output_postgres_db_instance_endpoint"></a> [postgres\_db\_instance\_endpoint](#output\_postgres\_db\_instance\_endpoint) | The connection endpoint |
| <a name="output_postgres_db_instance_engine"></a> [postgres\_db\_instance\_engine](#output\_postgres\_db\_instance\_engine) | The database engine |
| <a name="output_postgres_db_instance_engine_version_actual"></a> [postgres\_db\_instance\_engine\_version\_actual](#output\_postgres\_db\_instance\_engine\_version\_actual) | The running version of the database |
| <a name="output_postgres_db_instance_hosted_zone_id"></a> [postgres\_db\_instance\_hosted\_zone\_id](#output\_postgres\_db\_instance\_hosted\_zone\_id) | The canonical hosted zone ID of the DB instance (to be used in a Route 53 Alias record) |
| <a name="output_postgres_db_instance_identifier"></a> [postgres\_db\_instance\_identifier](#output\_postgres\_db\_instance\_identifier) | The RDS instance identifier |
| <a name="output_postgres_db_instance_name"></a> [postgres\_db\_instance\_name](#output\_postgres\_db\_instance\_name) | The database name |
| <a name="output_postgres_db_instance_port"></a> [postgres\_db\_instance\_port](#output\_postgres\_db\_instance\_port) | The database port |
| <a name="output_postgres_db_instance_resource_id"></a> [postgres\_db\_instance\_resource\_id](#output\_postgres\_db\_instance\_resource\_id) | The RDS Resource ID of this instance |
| <a name="output_postgres_db_instance_status"></a> [postgres\_db\_instance\_status](#output\_postgres\_db\_instance\_status) | The RDS instance status |
| <a name="output_postgres_db_instance_username"></a> [postgres\_db\_instance\_username](#output\_postgres\_db\_instance\_username) | The master username for the database |
| <a name="output_postgres_db_parameter_group_arn"></a> [postgres\_db\_parameter\_group\_arn](#output\_postgres\_db\_parameter\_group\_arn) | The ARN of the db parameter group |
| <a name="output_postgres_db_parameter_group_id"></a> [postgres\_db\_parameter\_group\_id](#output\_postgres\_db\_parameter\_group\_id) | The db parameter group id |
| <a name="output_postgres_db_subnet_group_arn"></a> [postgres\_db\_subnet\_group\_arn](#output\_postgres\_db\_subnet\_group\_arn) | The ARN of the db subnet group |
| <a name="output_postgres_db_subnet_group_id"></a> [postgres\_db\_subnet\_group\_id](#output\_postgres\_db\_subnet\_group\_id) | The db subnet group name |
<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
