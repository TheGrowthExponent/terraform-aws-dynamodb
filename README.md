# terraform-aws-dynamodb
Create a DynamoDB table with a primary key and secondary indexes.

## Usage
```hcl
module "dynamodb" {
  source     = "TheGrowthExponent/dynamodb/aws"
  version    = "1.0.0"
  table_name = "app-${var.application_name}-${var.environment}-ExampleTable"
  tags       = { purpose = "Application storage" }
}
```