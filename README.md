# Snowflake Terraform Task

## Purpose

This Terraform module is designed to provision a set of Snowflake resources including a warehouse, database, schema, table, and a role with specific privileges.
In this case, we will create a new user and grant a role to it right in the terraform. Otherwise a role can be granted manually to any other existing user.

## Prerequisites

- Terraform installed (https://developer.hashicorp.com/terraform/install)
- Snowflake account (https://signup.snowflake.com/)

## Configuration

1. Clone this repository.
2. Modify `terraform.tfvars` and `variables.tf` files, fill in your Snowflake credentials and desired resource names.
3. Run `terraform init` to initialize the Terraform configuration.
4. Run `terraform plan` to review the changes that will be made.
5. Run `terraform apply` to apply the changes to your Snowflake account.
6. Login as a newly creted user or grant the created role to any other user to check the functionality.

## Resources Created

- A Snowflake warehouse for query and data manipulation tasks.
- A dedicated Snowflake database.
- A schema within the database.
- A table within the schema with various data types.
- A role and a user with permissions for database, schema, and warehouse access, and select privileges on the table.

