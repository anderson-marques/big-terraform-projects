# Terraform Project Structure for Big Projects

For big projects with multi-cloud providers and dozens of resources are used. A good options is to create individual
files for each provider/resource type. That way, each file will contain only few lines of definitions and the whole
project becomes more manageable.

Example:

- `providers.tf` (Azure, AWS, Google, VMWare, etc...)
- `aws-s3.tf` - S3 buckets in aws.
