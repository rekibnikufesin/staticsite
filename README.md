#Hosting a static website on Amazon S3
This repo contains the website and bucket policy for my egghead.io lesson "Hosting a Static Website on Amazon S3"

Bucket policy:
```
{
  "Version":"2012-10-17",
  "Statement": [{
    "Sid": "Allow Public Access to All Objects",
    "Effect": "Allow",
    "Principal": "*",
    "Action": "s3:GetObject",
    "Resource": "arn:aws:s3:::staticsite.willbutton.co/*"
  }
 ]
}
```
