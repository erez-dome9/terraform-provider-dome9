---
layout: "dome9"
page_title: "Check Point CloudGuard Dome9: dome9_ruleset"
sidebar_current: "docs-datasource-dome9-ruleset"
description: |-
  Get information about a ruleset in Dome9.
---

# Data Source: dome9_ruleset

Use this data source to get information about a ruleset in Dome9.

## Example Usage

```hcl
data "dome9_ruleset" "test" {
  id        = "d9-rule-set-id"
}

```

## Argument Reference

The following arguments are supported:

* `id` - (Required) The id of the ruleset in Dome9.

## Attributes Reference

In addition to all arguments above, the following attributes are exported:

* `name	` - The ruleset name.
* `description` - The ruleset description.
* `cloud_vendor` - Cloud vendor that the ruleset is associated with.
* `created_time` - Rule set creation time.
* `updated_time` - Rule set last update time.
* `rules` - List of rules in the ruleset.
