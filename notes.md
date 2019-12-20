

Uses Serverless Framework

serverless -- Create new Lambda
serverless deploy -- upload to aws
serverelss dashboard -- monitor


https://github.com/aws-samples/lambda-refarch-mobilebackend


Stripe Integeration
https://serverless-stack.com/chapters/setup-a-stripe-account.html

Tools

Cognito - User poools for user login and managment.

app client id - 2lfvpds9e7kq9t8q1ht1bmtnvj

test User

API Gateway

Lambdas

Possible:
Serverless -




AWS Cognito Identity Pool Role

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": [
        "mobileanalytics:PutEvents",
        "cognito-sync:*",
        "cognito-identity:*"
      ],
      "Resource": [
        "*"
      ]
    },
    {
      "Effect": "Allow",
      "Action": [
        "s3:*"
      ],
      "Resource": [
        "arn:aws:s3:::equine-horse-app/private/${cognito-identity.amazonaws.com:sub}/*"
      ]
    },
    {
      "Effect": "Allow",
      "Action": [
        "execute-api:Invoke"
      ],
      "Resource": [
        "arn:aws:execute-api:us-east-2:*:m8nudfvxh0/*/*/*"
      ]
    }
  ]
}
