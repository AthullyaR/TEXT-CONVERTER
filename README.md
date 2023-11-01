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
- Add permission to role to perform operations on bucket.
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/ff9c56cd-191d-49a2-8758-3ac9f9132cb3)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/9451864a-6605-4259-95e6-d3549cefbcba)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/ebf6537c-6f28-41d7-916c-3e4c9be082b6)
![image](https://github.com/AthullyaR/TEXT-CONVERTER/assets/78737460/42885541-7617-49e1-af25-35d3299b28f4)



