# AWS-S3-Bucket-with-Python-boto3-
## Installation and setup

Step1 : Install boto3 using conda or pip on you PC / Laptop
conda install -c conda-forge boto3

ref: https://aws.amazon.com/sdk-for-python/

Step2 : provide user credentials to boto3
So do following steps

a. login to aws account

b. Go to services -> all services -> IAM service --> Users

c. Click create user

d. give the name

e. give access permissions to group

4 access permissions need to be give Search in filter following and enable them EC2 full access IAM full access S3 full access Route53 full access

f. create group

g. assign the permissions

h. logout

Step3. login go to iam service -> users
a. select the user to give programming access

b. click security credentials

c. Select access keys

d. Select use case local code

e. click on confirmation message

f. click next

g. click download csv file

h. click done

i. check in security credentials , access keys status is active

j. sign out

Step4. On your PC / laptop
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
