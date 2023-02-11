# Aws-Cli

issue: Can't Copy the whole bucket from Amazon s3 to desktop
using cli to to copy the bucket to desktop

DOWNLOAD aws cli software from aws website

step 1: use cmd and type aws--version (to check aws cli version)

step 2: aws configure to access your account through CLI, You need to provide access keys and Secret key

step 3: use aws s3 ls to see the bucket name

step 4: aws s3 sync s3://bucketname c/uses/desktop/website

All of your files will be saved in website folder which is located in desktop
