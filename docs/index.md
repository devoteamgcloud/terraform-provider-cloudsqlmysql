---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "cloudsqlmysql Provider"
subcategory: ""
description: |-
  The cloudsqlmysql provider makes it possible to grant permissions on MySQL databases and add rules for MySQL Audit Plugin. More info in the Google documentation https://cloud.google.com/sql/docs/mysql/db-audit.
---

# cloudsqlmysql Provider

The `cloudsqlmysql` provider makes it possible to grant permissions on MySQL databases and add rules for MySQL Audit Plugin. More info in the [Google documentation](https://cloud.google.com/sql/docs/mysql/db-audit).

## Example Usage

```terraform
terraform {
  required_providers {
    cloudsqlmysql = {
      source = "devoteamgcloud/cloudsqlmysql"
    }
  }
}

provider "cloudsqlmysql" {
  connection_name = "project:region:instance"
  username        = "root"
  password        = "password"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Optional

- `connection_name` (String) The connection name of the Google Cloud SQL MySQL instance
- `password` (String, Sensitive) The password to use to authenticate using the built-in database authentication
- `private_ip` (Boolean) Use the private IP address of the Cloud SQL MySQL instance to connect to
- `proxy` (String) Proxy socks url if used. Format needs to be `socks5://<ip>:<port>`
- `psc` (Boolean) Use the Private Service Connect endpoint of the Cloud SQL MySQL instance to connect to
- `username` (String) The username to use to authenticate with the Cloud SQL MySQL instance
