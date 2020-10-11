## Created a AWS Lambda Function to Send automated emails to the Users who requested for the Reciepe from the Web Application hosted on EC2 instance.

## Used the following AWS services along with Lambda

- SES
  - Simple Email Service to send emails
- SNS
  - Simple Notification Service will receive the tokens from dynamoDB and will push the information to SES to send email
- DynamoDB
  - Created a DynamoDB to generate a tokens when a user's request and push the token to SNS

## The user will only be able to request email only one time for a particular time frame.

    -   If a User request for a email more than 1 times in a timeframe of 5 minutes than also only one email will be sent to the user.

## CI/CD

    Created a CI/CD pipeline to deploy a new Lambda function or to Update an existing Lambda Function using Github and CircleCI
