# Hosting-a-static-webpage-using-s3-bucket-and-AWS-cloud-front

### Important steps to follow are highlighted below (with screenshots)

1. Sign in to AWS either as a root user or a IAM user but be sure the user has the required permissions to access the needed services i.e. s3 buckets and Cloudfront

2. Within the AWS console, search for s3 and create your bucket (follow all necessary steps)

   ![](Bucket_created.JPG)

3. Upload objects/files into your newly created s3 bucket

   ![](Folder_uploaded.JPG)

   ![](Bucket_and_its_content.JPG)

4. Move objects from the primary folder into the s3 bucket root folder

   ![](Objects_moved_to_the_s3_root_directory.JPG)

5. Now, create Cloudfront distribution to serve s3 bucket content

   ![](Cloudfront_distribution_created.JPG)

6. Ensure that the Cloudfront origin is set to your s3 bucket name

   ![](Origin_set_to_my_s3_bucket.JPG)

7. Now, update your s3 bucket policy to allow Cloudfront access to the objects/files to be served

   ![](s3_bucket_policy_edited_to_allow_cloudfront_principal_read_only_access.JPG)

   ![](s3_bucket_policy_content.JPG)

8. Now, copy your Cloudfront distribution domain name and paste in a browser to access the static webpage stored within the s3 bucket

   ![](Bucket_content_delivered_via_cloudfront_URL.JPG)

Now, you can access your webpage content hosted within an AWS s3 bucket via Cloudfront.
