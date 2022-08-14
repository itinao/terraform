## Terraform

## Rules
空でも下記ファイルを作成する
* `main.tf`
* `variables.tf`
* `outputs.tf`

そして、すべての `variable` `output` で description を定義すること

```terraform
variable "cidr_block" {
  description = "The CIDR block for the VPC."
}

output "vpc_id" {
  value       = aws_vpc.example.id
  description = "The ID of the VPC."
}
```

https://terraform-docs.io/

## Modular Design
Standard Module Structure

https://www.terraform.io/language/modules/develop/structure
