[![Follow on Twitter](https://img.shields.io/twitter/follow/opendevsecops.svg?logo=twitter)](https://twitter.com/opendevsecops)

# AWS Config Monitor Terraform Module

A terraform module to monitor Config with Slack and Email (soon).

## Getting Started

Getting started is easy. You will need Config provisioned via terraform or manually activated via the AWS console. Once Config is activated, simply import the module and configure as desired. Here is a complete example:

```terraform
module "config_monitor" {
  source = "opendevsecops/config-monitor/aws"

  monitor_slack_notification_url = "${var.monitor_slack_notification_url}"
}
```

The module is automatically published to the Terraform Module Registry. More information about the available inputs, outputs, dependencies and instructions how to use the module can be found at the official page [here](https://registry.terraform.io/modules/opendevsecops/config-monitor).
