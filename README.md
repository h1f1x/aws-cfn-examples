AWS example cloudformation templates
====================================

At the moment more a personal place to bootstrap infrastructure with cloudformation. Hopefully useful for anyone else too.
The examples a a little bit more than minimal and working with non-default ressources (e.g. non default VPC).

## EC2

The challenge here is to keep up-todate with the latest AMI.

Possible solutions:

- [AWS blogpost: Lambda for Lookup AMI Ids](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/walkthrough-custom-resources-lambda-lookup-amiids.html)
- [Using AWS SM Parameter Store for AMI Lookup](
https://aws.amazon.com/blogs/compute/query-for-the-latest-amazon-linux-ami-ids-using-aws-systems-manager-parameter-store/)

## ECR

 - [Cloudformation Docs: ECR](https://docs.aws.amazon.com/de_de/AWSCloudFormation/latest/UserGuide/aws-resource-ecr-repository.html)
 - [LifeCycle Policies (ECR)](https://docs.aws.amazon.com/AmazonECR/latest/userguide/lp_creation.html)

## DynamoDB

[Cloudformation Docs: DynamoDBTable](https://docs.aws.amazon.com/de_de/AWSCloudFormation/latest/UserGuide/aws-resource-dynamodb-table.html)

Challenge as of today is: restoring a cf managed table:
https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/backuprestore_HowItWorks.html
