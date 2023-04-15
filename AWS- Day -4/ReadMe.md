# Create a S3 bucket, with no public access and upload files to the bucket & view the logs using cloudwatch for the uploaded files. 

Step 1 : Login the amazon console login with your user name and password.

          https://console.aws.amazon.com/
          
Step 2 : Then select the S3 option from the menu and redirect to the page.

          https://s3.console.aws.amazon.com/s3/get-started?region=us-east-1

Step 3 : Click the Buckets option from the left side and it will take you to S3 bucket page, It shows the empty list on the right side.
          ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-s3-console-aws-amazon-s3-buckets-2023-04-15-11_48_11.png)
          

Stpe 4:  Click the create bucket and enter the S3 bucket information and verify the block all public access is enabled.
          ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-s3-console-aws-amazon-s3-bucket-create-2023-04-15-09_38_21.png)

Step 5: Enable the access log in S3 bucket.
         ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-s3-console-aws-amazon-s3-bucket-fghertyeryr-property-logging-edit-2023-04-15-12_08_44.png)

Step 6:  Upload the files in S3 bucket.
         ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-s3-console-aws-amazon-s3-upload-web-apps3-2023-04-15-09_40_44.png)

# Launch two ec2-instances and connect it to a application load balancer, where the output traffic from the server must be an load balancer IP address"
