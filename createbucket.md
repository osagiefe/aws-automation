
============================================
AWS Cli command for s3 
============================================

# Cmd to create bucket using aws cli
aws s3 mb s3://aws-lagos1 --region us-east-1

# Cmd to list bucket
aws s3 ls
# First delete all the objects present in given a bucket
aws s3 rm s3://gfg-example --recursive
# Cmd to remove bucket
aws s3 rb s3://aws-lagos1 --region us-east-1
aws s3 rb s3://aws-lagos1

============================================
AWS Cli command for IAM 
============================================
# Cmd to create IAM user
 aws iam create-user --user-name jack

# cmd to delete the IAM user
aws iam delete-user --user-name jack

# cmd to list IAM users
aws iam list-users

=======================================
# AWS cli for EC2 instance
=======================================
# cmd to create a keypair
aws ec2 create-key-pair --key-name boss --query 'KeyMaterial' --output text > boss.pem
chmod 400 boss.pem
# cmd to list/describe key pairs
aws ec2 describe-key-pairs