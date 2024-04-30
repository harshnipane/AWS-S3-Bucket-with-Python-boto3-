# AWS-S3-Bucket-with-Python-boto3-

It was fun to explore the combination of AWS S3 and Python's Boto3 library.

Boto3 is the Python SDK for AWS. It allows to directly create, update, and delete AWS resources like S3 from your Python scripts.

## Installation and setup

- Step1 : Install boto3 using conda or pip on you PC / Laptop
  conda install -c conda-forge boto3

  ref: https://aws.amazon.com/sdk-for-python/

- Step2 : provide user credentials to boto3
  So do following steps

  a. login to aws account

  c. Create user from IAM Service

  d. give access permissions to group

  e access permissions need to be give Search in filter following and enable them EC2 full access IAM full access S3 full access Route53 full access

  f. create group

  g. assign the permissions

  h. logout

- Step3. login go to iam service -> users
  a. select the user to give programming access

  b. click security credentials

  c. Select access keys

  d. Select use case local code

  e. click on confirmation message

  f. check in security credentials , access keys status is active

- Step4. On your PC / laptop
  a. create a directory AWS_S3

  b. copy the downloaded credentials CSV file

  c. create a .aws folder in 'C:\Users\your_user\' folder

  d. Inside .aws folder create file 'credentials' (without any extensions)

  e. paste crendentials in follwing format

  [default]

  aws_access_key_id = YOUR_ACCESS_KEY_ID

  aws_secret_access_key = YOUR_SECRET_ACCESS_KEY

  f. Inside .aws folder create file 'config' (without any extensions)

  g. paste region Mumbai in following format

  [default]

  region = ap-south-1

  h. Now default profile for boto3 is setup!

## Screenshots

Buckets created using boto3

![Screensho20](https://github.com/harshnipane/AWS-S3-Bucket-with-Python-boto3-/assets/85990319/511dc4e4-d18a-4452-95de-607d81e8d0f1)


Uploading File to S3 using python

![uploadfile](https://github.com/harshnipane/AWS-S3-Bucket-with-Python-boto3-/assets/85990319/4e523594-1b09-413a-a77b-7416655ebab1)


![Screenshot (21)](https://github.com/harshnipane/AWS-S3-Bucket-with-Python-boto3-/assets/85990319/ca6727d5-7efd-4327-8e2a-e24a1fea1eb3)

Deleting Buckets using python

![deletebuckets](https://github.com/harshnipane/AWS-S3-Bucket-with-Python-boto3-/assets/85990319/2cbaca08-0d81-410a-8896-0924b854a7db)
