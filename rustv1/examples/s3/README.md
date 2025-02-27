# Amazon S3 code examples for the SDK for Rust

## Overview

Shows how to use the AWS SDK for Rust to work with Amazon Simple Storage Service (Amazon S3).

<!--custom.overview.start-->
<!--custom.overview.end-->

_Amazon S3 is storage for the internet. You can use Amazon S3 to store and retrieve any amount of data at any time, from anywhere on the web._

## ⚠ Important

* Running this code might result in charges to your AWS account. For more details, see [AWS Pricing](https://aws.amazon.com/pricing/) and [Free Tier](https://aws.amazon.com/free/).
* Running the tests might result in charges to your AWS account.
* We recommend that you grant your code least privilege. At most, grant only the minimum permissions required to perform the task. For more information, see [Grant least privilege](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege).
* This code is not tested in every AWS Region. For more information, see [AWS Regional Services](https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services).

<!--custom.important.start-->
<!--custom.important.end-->

## Code examples

### Prerequisites

For prerequisites, see the [README](../../README.md#Prerequisites) in the `rustv1` folder.


<!--custom.prerequisites.start-->
<!--custom.prerequisites.end-->

### Single actions

Code excerpts that show you how to call individual service functions.

- [Complete a multipart upload](src/bin/s3-multipart-upload.rs#L138) (`CompleteMultipartUpload`)
- [Copy an object from one bucket to another](src/s3-service-lib.rs#L99) (`CopyObject`)
- [Create a bucket](src/s3-service-lib.rs#L156) (`CreateBucket`)
- [Create a multipart upload](src/bin/s3-multipart-upload.rs#L50) (`CreateMultipartUpload`)
- [Delete an empty bucket](src/s3-service-lib.rs#L25) (`DeleteBucket`)
- [Delete an object](src/bin/delete-object.rs#L32) (`DeleteObject`)
- [Delete multiple objects](src/s3-service-lib.rs#L33) (`DeleteObjects`)
- [Get an object from a bucket](src/bin/get-object.rs#L18) (`GetObject`)
- [Get an object from a bucket if it has been modified](src/bin/if-modified-since.rs#L6) (`GetObject`)
- [Get the Region location for a bucket](src/bin/list-buckets.rs#L28) (`GetBucketLocation`)
- [List buckets](src/bin/list-buckets.rs#L28) (`ListBuckets`)
- [List object versions in a bucket](src/bin/list-object-versions.rs#L28) (`ListObjectVersions`)
- [List objects in a bucket](src/s3-service-lib.rs#L73) (`ListObjectsV2`)
- [Upload a single part of a multipart upload](src/bin/s3-multipart-upload.rs#L114) (`UploadPart`)
- [Upload an object to a bucket](src/s3-service-lib.rs#L137) (`PutObject`)

### Scenarios

Code examples that show you how to accomplish a specific task by calling multiple
functions within the same service.

- [Create a presigned URL](src/bin/put-object-presigned.rs)
- [Get started with buckets and objects](src/bin/s3-getting-started.rs)
- [Upload or download large files](src/bin/s3-multipart-upload.rs)

### Cross-service examples

Sample applications that work across multiple AWS services.

- [Unit and integration test with an SDK](../../examples/testing)


<!--custom.examples.start-->
<!--custom.examples.end-->

## Run the examples

### Instructions


<!--custom.instructions.start-->
<!--custom.instructions.end-->



#### Create a presigned URL

This example shows you how to create a presigned URL for Amazon S3 and upload an object.


<!--custom.scenario_prereqs.s3_Scenario_PresignedUrl.start-->
<!--custom.scenario_prereqs.s3_Scenario_PresignedUrl.end-->


<!--custom.scenarios.s3_Scenario_PresignedUrl.start-->
<!--custom.scenarios.s3_Scenario_PresignedUrl.end-->

#### Get started with buckets and objects

This example shows you how to do the following:

- Create a bucket and upload a file to it.
- Download an object from a bucket.
- Copy an object to a subfolder in a bucket.
- List the objects in a bucket.
- Delete the bucket objects and the bucket.

<!--custom.scenario_prereqs.s3_Scenario_GettingStarted.start-->
<!--custom.scenario_prereqs.s3_Scenario_GettingStarted.end-->


<!--custom.scenarios.s3_Scenario_GettingStarted.start-->
<!--custom.scenarios.s3_Scenario_GettingStarted.end-->

#### Upload or download large files

This example shows you how to upload or download large files to and from Amazon S3.


<!--custom.scenario_prereqs.s3_Scenario_UsingLargeFiles.start-->
<!--custom.scenario_prereqs.s3_Scenario_UsingLargeFiles.end-->


<!--custom.scenarios.s3_Scenario_UsingLargeFiles.start-->
<!--custom.scenarios.s3_Scenario_UsingLargeFiles.end-->

### Tests

⚠ Running tests might result in charges to your AWS account.


To find instructions for running these tests, see the [README](../../README.md#Tests)
in the `rustv1` folder.



<!--custom.tests.start-->
<!--custom.tests.end-->

## Additional resources

- [Amazon S3 User Guide](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)
- [Amazon S3 API Reference](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html)
- [SDK for Rust Amazon S3 reference](https://docs.rs/aws-sdk-s3/latest/aws_sdk_s3/)

<!--custom.resources.start-->
<!--custom.resources.end-->

---

Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.

SPDX-License-Identifier: Apache-2.0