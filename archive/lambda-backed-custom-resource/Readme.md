- Sort image by time: `aws ec2 describe-images --filter Name=name,Values=amzn-ami-*-amazon-ecs-optimized --profile dacn --query 'sort_by(Images, &CreationDate)[]'`

# Reference

1. [Query for the latest Amazon Linux AMI IDs using AWS Systems Manager Parameter Store](https://aws.amazon.com/blogs/compute/query-for-the-latest-amazon-linux-ami-ids-using-aws-systems-manager-parameter-store/)
