---
subcategory: "AMP (Managed Prometheus)"
layout: "aws"
page_title: "AWS: aws_prometheus_workspace"
description: |-
  Gets information on an Amazon Managed Prometheus workspace.
---

# Data Source: aws_amp_workspace

Provides an Amazon Managed Prometheus workspace data source.

## Example Usage

### Basic configuration

```terraform
data "aws_amp_workspace" "example" {
  workspace_id = "ws-41det8a1-2c67-6a1a-9381-9b83d3d78ef7"
}
```

## Argument Reference

The following arguments are required:

* `workspace_id` - (Required) Prometheus workspace ID.

## Attributes Reference

In addition to all arguments above, the following attributes are exported:

* `arn` - ARN of the Prometheus workspace.
* `created_date` - Creation date of the Prometheus workspace.
* `prometheus_endpoint` - Endpoint of the Prometheus workspace.
* `alias` - Prometheus workspace alias.
* `status` - Status of the Prometheus workspace.
* `tags` - Tags assigned to the resource.
