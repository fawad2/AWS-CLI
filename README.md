# Aws-Cli

issue: Can't Copy the whole bucket from Amazon s3 to desktop
using cli to to copy the bucket to desktop

DOWNLOAD aws cli software from aws website

step 1: use cmd and type aws--version (to check aws cli version)

step 2: aws configure to access your account through CLI, You need to provide access keys and Secret key

step 3: use aws s3 ls to see the bucket name

step 4: aws s3 sync s3://bucketname c/uses/desktop/website

All of your files will be saved in website folder which is located in desktop

How to see files in aws s3 bucket
First of all open aws cli -> aws configure -> login -> aws s3 ls (to find a bucket name)
to see files and folders in bucket -> aws s3 ls s3://mybucket (this command will show folder name but not files under it)

to see all the files inside folders in bucket

type: aws s3 ls s3://mybucket --recursive

To see the size of your bucket/files in the bucket, use:
aws s3 ls s3://mybucket --recursive --human-readable --summarize

How do I create an IAM user from CLI?

Step: 1 configure
Step 2: aws iam create-user --user-name fawad2
User is created

How do I remove an IAM user from the CLI?
Ans: aws iam delete-user --user-name fawad2

How to create a password for iam user ?
aws iam create-login-profile --user-name fawad --password yourpassword
