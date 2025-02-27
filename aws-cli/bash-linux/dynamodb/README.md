# DynamoDB code examples for the AWS CLI with Bash script

## Overview

Shows how to use the AWS Command Line Interface with Bash script to work with Amazon DynamoDB.

<!--custom.overview.start-->
<!--custom.overview.end-->

_DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability._

## ⚠ Important

* Running this code might result in charges to your AWS account. For more details, see [AWS Pricing](https://aws.amazon.com/pricing/) and [Free Tier](https://aws.amazon.com/free/).
* Running the tests might result in charges to your AWS account.
* We recommend that you grant your code least privilege. At most, grant only the minimum permissions required to perform the task. For more information, see [Grant least privilege](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege).
* This code is not tested in every AWS Region. For more information, see [AWS Regional Services](https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services).

<!--custom.important.start-->
<!--custom.important.end-->

## Code examples

### Prerequisites

For prerequisites, see the [README](../../README.md#Prerequisites) in the `aws-cli` folder.


<!--custom.prerequisites.start-->
<!--custom.prerequisites.end-->

### Single actions

Code excerpts that show you how to call individual service functions.

- [Create a table](dynamodb_operations.sh#L23) (`CreateTable`)
- [Delete a table](dynamodb_operations.sh#L1004) (`DeleteTable`)
- [Delete an item from a table](dynamodb_operations.sh#L541) (`DeleteItem`)
- [Get a batch of items](dynamodb_operations.sh#L908) (`BatchGetItem`)
- [Get an item from a table](dynamodb_operations.sh#L445) (`GetItem`)
- [Get information about a table](dynamodb_operations.sh#L189) (`DescribeTable`)
- [List tables](dynamodb_operations.sh#L975) (`ListTables`)
- [Put an item in a table](dynamodb_operations.sh#L263) (`PutItem`)
- [Query a table](dynamodb_operations.sh#L620) (`Query`)
- [Scan a table](dynamodb_operations.sh#L730) (`Scan`)
- [Update an item in a table](dynamodb_operations.sh#L344) (`UpdateItem`)
- [Write a batch of items](dynamodb_operations.sh#L840) (`BatchWriteItem`)

### Scenarios

Code examples that show you how to accomplish a specific task by calling multiple
functions within the same service.

- [Get started with tables, items, and queries](scenario_getting_started_movies.sh)


<!--custom.examples.start-->
<!--custom.examples.end-->

## Run the examples

### Instructions


<!--custom.instructions.start-->
<!--custom.instructions.end-->



#### Get started with tables, items, and queries

This example shows you how to do the following:

- Create a table that can hold movie data.
- Put, get, and update a single movie in the table.
- Write movie data to the table from a sample JSON file.
- Query for movies that were released in a given year.
- Scan for movies that were released in a range of years.
- Delete a movie from the table, then delete the table.

<!--custom.scenario_prereqs.dynamodb_Scenario_GettingStartedMovies.start-->
<!--custom.scenario_prereqs.dynamodb_Scenario_GettingStartedMovies.end-->


<!--custom.scenarios.dynamodb_Scenario_GettingStartedMovies.start-->
<!--custom.scenarios.dynamodb_Scenario_GettingStartedMovies.end-->

### Tests

⚠ Running tests might result in charges to your AWS account.


To find instructions for running these tests, see the [README](../../README.md#Tests)
in the `aws-cli` folder.



<!--custom.tests.start-->
<!--custom.tests.end-->

## Additional resources

- [DynamoDB Developer Guide](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html)
- [DynamoDB API Reference](https://docs.aws.amazon.com/amazondynamodb/latest/APIReference/Welcome.html)
- [AWS CLI with Bash script DynamoDB reference](https://awscli.amazonaws.com/v2/documentation/api/latest/reference/dynamodb/index.html)

<!--custom.resources.start-->
<!--custom.resources.end-->

---

Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.

SPDX-License-Identifier: Apache-2.0