# Cost Estimation

cost estimation for an attendance management system using AWS services for an institution with 20,000 students and 1,000 sections per semester :
1. EC2 Instances:
- The institution requires 10 ‘m5.large’ instances to handle the expected load.
- The hourly cost of an ‘m5.large’ instance is $0.096.
- Assuming the system is used 24 hours a day, 5 days a week, and 22 days a month (excluding weekends), the monthly cost for EC2 instances would be: $0.096 * 10 * 24 * 22 = $5,068.
2. S3 Storage:
- The attendance management system requires 500GB of S3 storage.
- The cost per GB of S3 storage is $0.023.
- The monthly cost for S3 storage would be: $0.023 * 500 = $11.50.
3. DynamoDB Provisioned Capacity:
- The attendance management system requires provisioned capacity of 500 read capacity units and 100 write capacity units.
- The cost per read capacity unit is $0.00013 and the cost per write capacity unit is $0.00065.
- The monthly cost for DynamoDB provisioned capacity would be: ($0.00013 * 500) + ($0.00065 * 100) = $0.065 + $0.065 = $0.13.
4. Lambda Function Invocations:
- The attendance management system has an estimated 100,000 Lambda function invocations per month.
- The cost per invocation is $0.0000002.
- The monthly cost for Lambda function invocations would be: $0.0000002 * 100,000 = $0.02.
5. API Gateway Usage:
- The attendance management system has an estimated 1,000,000 API Gateway requests per month.
- The cost per request is $0.000001.
- The monthly cost for API Gateway usage would be: $0.000001 * 1,000,000 = $1.
6. CloudFront Distribution:
- The attendance management system has an estimated 100GB of data transferred through CloudFront per month.
- The cost per GB transferred is $0.085.
- The monthly cost for CloudFront distribution would be: $0.085 * 100 = $8.50.

7.Total Monthly Cost:
- Summing up the individual costs: $5,068 + $11.50 + $0.13 + $0.02 + $1 + $8.50 = $5,089.15
