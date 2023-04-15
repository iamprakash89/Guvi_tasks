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

Step 1: Create a Two instances from EC2 launch instance
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-us-east-1-console-aws-amazon-ec2-home-2023-04-15-09_00_04.png)
       ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-us-east-1-console-aws-amazon-ec2-home-2023-04-15-09_00_18.png)
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-us-east-1-console-aws-amazon-ec2-home-2023-04-15-09_00_29.png)
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-us-east-1-console-aws-amazon-ec2-home-2023-04-15-09_01_57.png)

Step 2: Before creating a Loadbalancer, we need to create a Target groups. this target groups contians the Ec2 instances which is going to handled by Load balancer.
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-us-east-1-console-aws-amazon-ec2-home-2023-04-15-09_03_11.png)
Step 3: Add your Target resources ion your Target group        
        ![alt text](![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-us-east-1-console-aws-amazon-ec2-home-2023-04-15-09_04_32.png)
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-us-east-1-console-aws-amazon-ec2-home-2023-04-15-09_05_10.png)
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-us-east-1-console-aws-amazon-ec2-home-2023-04-15-09_05_47.png)
 
Step 4: Now create your load balancer and add your Target groups.
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-us-east-1-console-aws-amazon-ec2-home-2023-04-15-09_09_10.png)

Step 5: Create a Security group for LB and EC2 instances
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-us-east-1-console-aws-amazon-ec2-home-2023-04-15-09_26_24.png)
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/screencapture-us-east-1-console-aws-amazon-ec2-home-2023-04-15-09_26_57.png)
 
Step 6: Installing a apache and add some index file in the server end.
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/putty.PNG)
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/putty2.PNG)
       
Step 7: Verifying the Server website has been accessed from the public.
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/server1.PNG)
        ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/server2.PNG)
        
Step 8: Verify from the load balancer with the website
         ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/LB-1.PNG)
         ![alt text](https://github.com/iamprakash89/Guvi_tasks/blob/main/AWS-%20Day%20-4/images/LB-2.PNG)
