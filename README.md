In this AWS tutorial, I’ll show you how to create IAM users with restricted EC2-only permissions — one with Console Access and another with Programmatic (CLI) Access. This is a core DevOps and Cloud skill used in real companies and perfect for beginners, interns, and job seekers.

🔥 What you will learn in this :

How to create an IAM user from the AWS root account

How to enable console login

How to create a Programmatic IAM user

How to attach a custom EC2-only policy

How to log in using the IAM console URL

How to configure AWS CLI using access keys

How to test EC2 allowed/denied actions

How to safely delete IAM users

MUST-know AWS security best practices

📌 Custom IAM Policy Used in This Video
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": "ec2:*",
      "Resource": "*"
    }
  ]
}


This policy gives full EC2 access only and blocks all other AWS services.

💻 AWS CLI Commands Used
🔹 Configure AWS CLI
aws configure

🔹 Verify IAM Identity
aws sts get-caller-identity

🔹 Describe EC2 Instances (Should work)
aws ec2 describe-instances

🔹 S3 Access Test (Should fail)
aws s3 ls

🧠 Why This Task Is Important

IAM + EC2 access control is one of the most fundamental cloud security topics every DevOps and Cloud engineer must understand. The “least privilege model” is used in all real companies to protect AWS accounts from misuse.

This video helps you build:
✔ Real AWS skills
✔ A strong resume project
✔ Internship/college report content
✔ A portfolio piece for GitHub and LinkedIn

💡 Useful Topics Covered

IAM User

Console Access

Access Keys

AWS CLI

EC2 management

Security credentials

Permissions boundary

Role-based access control

❤️ Support the Channel

https://youtu.be/ceqSTsFT7xs?si=wMeUuJB5-gSgO0f3
