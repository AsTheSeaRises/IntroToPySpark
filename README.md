# Intro To PySpark

The purpose of these snippets of code and scripts, are to make it easier to launch PySpark on Amazon EMR, while using a Jupyter Notebook style approach to learning the basics of Spark. Following this approach will allow you to have a permanent or peristent notebook saved in Amazon S3 for use with transient EMR clusters.

Configuration based on https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-jupyterhub-s3.html

# Prerequisites
1) AWS account (sign up) https://aws.amazon.com/

# Steps Required
Process to launch EMR cluster with PySpark and JupyterHub installed, along with pre-created Jupyter notebook to get you started.
## Step 1 - Create bucket that will contain your saved notebooks
Log into the AWS console https://aws.amazon.com/
Create a S3 bucket


Copy the notebook into this bucket
## Step 2 - Create bucket that will contain the shell script used during EMR launch
Copy 'findspark.sh' into this bucket.
## Step 3 - Run EMR create cluster from CLI
CLI command can be found at IntroToPySpark/CLI_Launch
      
