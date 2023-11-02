# TEXT-CONVERTER

## Overview
Services used in the project:

![services](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/3706f75d-d6aa-4e77-8047-7384f155ab2d)

## Description
TEXT-CONVERTER converts the text entered by the user into speech using AWS polly service. On submitting the user input, AWS Lambda function is triggered by the API Endpoint generated using API Gateway. In the AWS Lambda function, code is written to convert text to speech using AWS Polly and store it into Amazon S3 bucket. Later, stored S3 bucket object is retrieved and a presigned url is generated and send as the response.

## Step 1: Create S3 bucket
- Go tp Amazon S3 in the console.
- Create the bucket to upload the converted speech.
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/8b75fd76-da6f-46fe-affd-6894ea618833)

## Step 2 : Creating AWS Lambda function
- Go to AWS Lambda in the console.
- Create the Lambda function by specifying name and env.
- Write the code, save and deploy. Test the function by configuring a test event.
- Add permission to access synthesize_speech (polly).
- Add permission to role to perform operations on bucket (inline policy).
- Inorder to access the object URL in Amazon S3, need to allow public access.
- Go to permissions and edit the block public access and also add the bucket policy.
- Use the polly (synthesize_speech) to convert text to speech in the code.
- Test the Lambda function to see the working.
  
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/ff9c56cd-191d-49a2-8758-3ac9f9132cb3)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/9451864a-6605-4259-95e6-d3549cefbcba)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/ebf6537c-6f28-41d7-916c-3e4c9be082b6)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/42885541-7617-49e1-af25-35d3299b28f4)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/3fe48a5c-e2db-4430-9c2b-db932bad3f09)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/18497c8c-84d3-4ac2-9ef2-80f65393a848)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/8b0d40fd-bdc3-4646-a252-227ebf4fdc6e)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/5926fd78-f184-4322-95d9-c186fe769284)

## Step 3: Creating API using API Gateway
- Go to Amazon API Gateway in the console.
- Build a REST API, create resource and method by specifying the method type and lambda function.
- Enable CORS to access from browser (choose the resouce created to view the enable cors option).
- Test to see the working and deploy API.
- Fetch the API endpoint from AWS Lambda console and use it to trigger the AWS Lambda function.

![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/dba1259b-a02e-4834-9623-d7a86e60faae)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/a76c83f6-6c06-4e05-8c84-29f557e7f6b6)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/d8613dc6-5d5b-427e-b96b-2d1ca5be2dd2)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/d648f8df-431c-4a57-8382-b521951dc162)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/73fa2888-7a0d-48bb-acfb-45d64d7a2d4d)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/c16a89b6-b3c2-4a1a-83b9-a6683ba94a8a)

## Step 4: Deploy using AWS Amplify
- Go to AWS Amplify console and choose host app.
- Drag and drop the html file and deploy.

![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/fd5c52a2-026f-4688-8f49-24ae74887831)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/15b14634-231f-4952-8506-1c0166c4331f)

















