---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "cloudsqlmysql_grant_database Resource - cloudsqlmysql"
subcategory: ""
description: |-
  
---

# cloudsqlmysql_grant_database (Resource)



## Example Usage

```terraform
resource "cloudsqlmysql_database_grant" "default" {
  database          = "database"
  user              = "user"
  privileges        = ["SELECT", "UPDATE", "DELETE"]
  with_grant_option = true
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `database` (String)
- `privileges` (Set of String)

### Optional

- `host` (String)
- `role` (String)
- `user` (String)
- `with_grant_option` (Boolean)
