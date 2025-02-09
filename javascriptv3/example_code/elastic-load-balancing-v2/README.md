# ELB code examples for the SDK for JavaScript (v3)

## Overview

Shows how to use the AWS SDK for JavaScript (v3) to work with Elastic Load Balancing (ELB).

<!--custom.overview.start-->
<!--custom.overview.end-->

_ELB automatically distributes your incoming traffic across multiple targets, such as EC2 instances, containers, and IP addresses, in one or more Availability Zones._

## ⚠ Important

* Running this code might result in charges to your AWS account. For more details, see [AWS Pricing](https://aws.amazon.com/pricing/) and [Free Tier](https://aws.amazon.com/free/).
* Running the tests might result in charges to your AWS account.
* We recommend that you grant your code least privilege. At most, grant only the minimum permissions required to perform the task. For more information, see [Grant least privilege](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege).
* This code is not tested in every AWS Region. For more information, see [AWS Regional Services](https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services).

<!--custom.important.start-->
<!--custom.important.end-->

## Code examples

### Prerequisites

For prerequisites, see the [README](../../README.md#Prerequisites) in the `javascriptv3` folder.


<!--custom.prerequisites.start-->
<!--custom.prerequisites.end-->

### Get started

- [Hello Elastic Load Balancing](javascriptv3/example_code/elastic-load-balancing-v2/hello.js) (`DescribeLoadBalancers`)


### Single actions

Code excerpts that show you how to call individual service functions.

- [Create a listener for a load balancer](../cross-services/wkflw-resilient-service/steps-deploy.js#L465) (`CreateListener`)
- [Create a target group](../cross-services/wkflw-resilient-service/steps-deploy.js#L404) (`CreateTargetGroup`)
- [Create an Application Load Balancer](../cross-services/wkflw-resilient-service/steps-deploy.js#L437) (`CreateLoadBalancer`)
- [Delete a load balancer](../cross-services/wkflw-resilient-service/steps-destroy.js#L295) (`DeleteLoadBalancer`)
- [Delete a target group](../cross-services/wkflw-resilient-service/steps-destroy.js#L329) (`DeleteTargetGroup`)
- [Describe target groups](../cross-services/wkflw-resilient-service/steps-demo.js#L79) (`DescribeTargetGroups`)
- [Get the endpoint of a load balancer](javascriptv3/example_code/elastic-load-balancing-v2/hello.js) (`DescribeLoadBalancers`)
- [Get the health of a target group](../cross-services/wkflw-resilient-service/steps-demo.js#L88) (`DescribeTargetHealth`)

### Scenarios

Code examples that show you how to accomplish a specific task by calling multiple
functions within the same service.

- [Build and manage a resilient service](javascriptv3/example_code/cross-services/wkflw-resilient-service/index.js)


<!--custom.examples.start-->
<!--custom.examples.end-->

## Run the examples

### Instructions

**Note**: All code examples are written in ECMAscript 6 (ES6). For guidelines on converting to CommonJS, see
[JavaScript ES6/CommonJS syntax](https://docs.aws.amazon.com/sdk-for-javascript/v3/developer-guide/sdk-examples-javascript-syntax.html).

**Run a single action**

```bash
node ./actions/<fileName>
```

**Run a scenario**
Most scenarios can be run with the following command:
```bash
node ./scenarios/<fileName>
```

<!--custom.instructions.start-->
<!--custom.instructions.end-->

#### Hello Elastic Load Balancing

This example shows you how to get started using Elastic Load Balancing.

```bash
node ./hello.js
```


#### Build and manage a resilient service

This example shows you how to create a load-balanced web service that returns book, movie, and song recommendations. The example shows how the service responds to failures, and how to restructure the service for more resilience when failures occur.

- Use an Amazon EC2 Auto Scaling group to create Amazon Elastic Compute Cloud (Amazon EC2) instances based on a launch template and to keep the number of instances in a specified range.
- Handle and distribute HTTP requests with Elastic Load Balancing.
- Monitor the health of instances in an Auto Scaling group and forward requests only to healthy instances.
- Run a Python web server on each EC2 instance to handle HTTP requests. The web server responds with recommendations and health checks.
- Simulate a recommendation service with an Amazon DynamoDB table.
- Control web server response to requests and health checks by updating AWS Systems Manager parameters.

<!--custom.scenario_prereqs.cross_ResilientService.start-->
<!--custom.scenario_prereqs.cross_ResilientService.end-->


<!--custom.scenarios.cross_ResilientService.start-->
<!--custom.scenarios.cross_ResilientService.end-->

### Tests

⚠ Running tests might result in charges to your AWS account.


To find instructions for running these tests, see the [README](../../README.md#Tests)
in the `javascriptv3` folder.



<!--custom.tests.start-->
<!--custom.tests.end-->

## Additional resources

- [ELB User Guide](https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/what-is-load-balancing.html)
- [ELB API Reference](https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/Welcome.html)
- [SDK for JavaScript (v3) ELB reference](https://docs.aws.amazon.com/AWSJavaScriptSDK/v3/latest/client/elastic-load-balancing-v2)

<!--custom.resources.start-->
<!--custom.resources.end-->

---

Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.

SPDX-License-Identifier: Apache-2.0