# Serving static content: AWS Edition

**-TLDR-** This blog explains how to store static content in the cloud in a secure manner and how to access it through your own domain! 

You ever wanted to store pictures of cat hats in the cloud but never had the time to figure out how? In a few easy steps we will explain how! In this tutorial we will explain how to store static content in AWS S3 Buckets, how to handle the permissions, how to make the files __*BLAZINGLY*__ fast to load and how to use your own domain to access them!

1. **S3 - Cloud Storage**
2. CloudFront - Serve S3 content from cached edge locations 
3. Route53 - Use your own domain
4. Certificate Manager - Seal of approval

## S3 - Cloud Storage
The first step into building our cat hats vault is setting up AWS S3. What is S3? 
> Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. 

What does this mean for us? It means we found the perfect place to store our pictures as it provides high availability at a very cheap price. In S3 data is stored in buckets. Let's create our first one:
![s3](assets/s3.png "AWS S3")
1. Go to Services - top left corner, and click on S3, you might have to search for it
2. Create new bucket by clicking on the Create Bucket orange button - keep the recommended settings including block from public access. Try to give it a meaningful name. Once created you should see it in the bucket list.
3. (Optional) Upload some sample pictures by clicking on the Upload button

Great progress! We now are ready to store infinite amount of cat hat pictures! Let's now make them accessible through AWS Cloudfront so we have the 


