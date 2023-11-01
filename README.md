# TEXT-CONVERTER

##Step 1: Create S3 bucket
- Go tp Amazon S3 in the console.
- Create the bucket to upload the converted speech.
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/f6702c83-3e47-4da8-b428-b1694587ccba)

##Step 2 : Creating AWS Lambda function
- Go to AWS Lambda in the console.
- Create the Lambda function by specifying name and env.
- Write the code, save and deploy. Test the function by configuring a test event.
- Add permission to access synthesize_speech (polly).
- Add permission to role to perform operations on bucket (inline policy).
- Inorder to access the object URL in Amazon S3, need to allow public access.
- Go to permissions and edit the block public access and also add the bucket policy.
  
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/ff9c56cd-191d-49a2-8758-3ac9f9132cb3)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/9451864a-6605-4259-95e6-d3549cefbcba)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/ebf6537c-6f28-41d7-916c-3e4c9be082b6)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/42885541-7617-49e1-af25-35d3299b28f4)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/3fe48a5c-e2db-4430-9c2b-db932bad3f09)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/18497c8c-84d3-4ac2-9ef2-80f65393a848)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/8b0d40fd-bdc3-4646-a252-227ebf4fdc6e)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/5926fd78-f184-4322-95d9-c186fe769284)

##Step 3: Creating API using API Gateway
- Go to Amazon API Gateway in the console.
- Build a REST API and create method.

![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/dba1259b-a02e-4834-9623-d7a86e60faae)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/5b5ac960-9391-4c66-bd4e-54b4e04c1530)









