# Release-to-S3
Proof of concept application that gets automatically uploaded to AWS S3 when a release is made  
  
### How it works
Whenever a release is published, a webhook will call an AWS Lambda that will gather the release files' browser_download_url's. It will then download the files and store them as objects in an AWS S3 bucket.
