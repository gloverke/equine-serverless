


-- Cognito --

App Client ID 2lfvpds9e7kq9t8q1ht1bmtnvj
User Pool ID us-east-2_CRQ8aCfRK
test user
admin@example.com
abc123DEF

Create a user
aws cognito-idp sign-up \
 --region YOUR_COGNITO_REGION \
 --client-id YOUR_COGNITO_APP_CLIENT_ID \
 --username admin@example.com \
 --password Passw0rd!

 Confirm user
 aws cognito-idp admin-confirm-sign-up \
  --region YOUR_COGNITO_REGION \
  --user-pool-id YOUR_COGNITO_USER_POOL_ID \
  --username admin@example.com



--  Serverless ---

Kickstart a service
serverless install --url https://github.com/AnomalyInnovations/serverless-nodejs-starter --name <NAME>


npm install
npm install aws-sdk --save-dev
npm install uuid --save
