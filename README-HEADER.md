# PBS TF SNS Topic Subscription Module

## Installation

### Using the Repo Source

Use this URL for the source of the module. See the usage examples below for more details.

```hcl
github.com/pbs/terraform-aws-sns-topic-subscription-module?ref=x.y.z
```

### Alternative Installation Methods

More information can be found on these install methods and more in [the documentation here](./docs/general/install).

## Usage

Subscribes an endpoint to an SNS topic.

Integrate this module like so:

```hcl
module "subscription" {
  source = "github.com/pbs/terraform-aws-sns-topic-subscription-module?ref=x.y.z"

  topic_arn = module.topic.arn
  protocol  = "lambda"
  endpoint  = module.lambda.arn
}
```

## Adding This Version of the Module

If this repo is added as a subtree, then the version of the module should be close to the version shown here:

`x.y.z`

Note, however that subtrees can be altered as desired within repositories.

Further documentation on usage can be found [here](./docs).

Below is automatically generated documentation on this Terraform module using [terraform-docs][terraform-docs]

---

[terraform-docs]: https://github.com/terraform-docs/terraform-docs