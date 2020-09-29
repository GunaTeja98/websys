# README

Deploy a sample Photosite Rails Application to AWS via Docker
In this project, we will create a Ruby on Rails application that implements only a part of a Photo Sharing site specifically only the comments section with data that already entered into a SQL-Lite database.


1. Youtube walkThrough


2. Develop the Photosite app with the image files stored in AWS S3 services.
All the necessary data related to the photosite application should be stored under the SQL-Lite database. Configure the rails application and make sure it is connected to the database successfully. The core logic needs to be implemented.
Host Images on Amazon S3 and access the image using a generated public link in code.
Steps to host the images on S3 are listed below:
Create S3 Bucket
Click Create Bucket, enter the name, and select Region: US Standard


Upload files to the S3 Bucket
Once created, click on the bucket name in the list on the left and then click Upload on the next screen


Add an S3 Bucket policy
In the Bucket name list, choose the name of the bucket that you want to create a bucket policy for or whose bucket policy you wantto edit.

Choose Permissions, and then choose Bucket Policy.

In the Bucket policy editor text box, type or copy and paste a new bucket policy, or edit an existing policy. The bucket policy is a JSON file. The text you type in the editor must be valid JSON.

Choose Save.





Get the public link of an object(image) from an S3 bucket in the following way:
In the Name list, select the check box next to the object you want to get the public link, and then copy the lonk on the object description page that appears.


Once everything is in place run the application and verify it by hitting the URL http://localhost:3000/. It should display a list of all users in the database. The user names must be links and by clicking on a user name should display the photos for that user.

