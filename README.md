# Intro To PySpark

The purpose of these snippets of code and scripts, are to make it easier to launch PySpark on Amazon EMR, while using a Jupyter Notebook style approach to learning the basics of Spark. Following this approach will allow you to have a permanent or peristent notebook saved in Amazon S3 for use with transient EMR clusters.

Configuration based on https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-jupyterhub-s3.html

# Prerequisites
1) AWS account (sign up) https://aws.amazon.com/

# Steps Required
Process to launch EMR cluster with PySpark and JupyterHub installed, along with pre-created Jupyter notebook to get you started.
## Step 1 - Create bucket that will contain your saved notebooks
a) Log into the AWS console https://aws.amazon.com/

To create an S3 bucket

    Sign in to the AWS Management Console and open the Amazon S3 console at https://console.aws.amazon.com/s3/.


![alt text](https://docs.aws.amazon.com/AmazonS3/latest/gsg/images/create-bucket.png)




b) In the Bucket name field, type a unique DNS-compliant name for your new bucket. (The example screen shot uses the bucket name admin-created. You cannot use this name because S3 bucket names must be unique.) Create your own bucket name using the follow naming guidelines:

    The name must be unique across all existing bucket names in Amazon S3.

    After you create the bucket you cannot change the name, so choose wisely.

    Choose a bucket name that reflects the objects in the bucket because the bucket name is visible in the URL that points to the objects that you're going to put in your bucket.

For information about naming buckets, see Rules for Bucket Naming in the Amazon Simple Storage Service Developer Guide.

For Region, choose US West (Oregon) as the region where you want the bucket to reside.

c) Choose Create.

![alt text] https://docs.aws.amazon.com/AmazonS3/latest/gsg/images/gsg-create-bucket-name-region.png



Copy the notebook into this bucket
## Step 2 - Create bucket that will contain the shell script used during EMR launch
Copy 'findspark.sh' into this bucket.
## Step 3 - Run EMR create cluster from CLI
CLI command can be found at IntroToPySpark/CLI_Launch
      
