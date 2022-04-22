# AWS-S3-API-bucket-playground

This repo holds a Postman collection to:

* Create a bucket
* Add tags to a Bucket
* Check if a bucket has tags
* Check if a bucket is encrypted
* Check if a bucket has a IAM policy
* Add Encryption a bucket
* Add IAM Policy to a bucket
* Create a Cloud trail
* Check Cloud trail for ConsoleLogin events and create an array of source IPs
* Check IP Addresses' reputation against Virustotal api
* delete cloud trail
* delete bucket

![ Overview ](./Assets/overview.png "Overview")


## Pre requisites

[AWS access key](https://aws.amazon.com/premiumsupport/knowledge-center/create-access-key/) and [Virustotal API key](https://developers.virustotal.com/reference/getting-started) will be needed.

### Add Collection to Postman

 To import this colletion to your postman, go to File -> Import (Ctrl - O)

![ File -> Import](./Assets/file_import.png "File -> Import")

 Then choose link , and add the raw link to the Collection in this repo:

  https://raw.githubusercontent.com/guybli/S3-bucket-playground/main/AWS_S3_BUCKET_API.postman_collection.json

![Import Collection](./Assets/import_collection.png "Import Collection")

 Then you should be able to see the Collection in Postman
![Collection in Postman](./Assets/collection_added.png "Collection in Postman")


### Add Variables

This collection requires certain variables to work:

* IP_ADDRESS (Auto Populated)
* IP_ADDRESSES (Auto Populated)
* BUCKET_NAME
* AWS_REGION
* AWS_ACCESS_KEY
* AWS_SECRET_KEY
* AWS_SESSION_TOKEN
* AWS_SESSION_EXPIRATION
* VIRUSTOTAL_API_KEY
* CLOUD_TRAIL_NAME
* AWS_ACCOUNT_ID
* BUCKET_OBJECT_KEY (Auto Populated)

These can be added from the *Variables* Tab of the Collection:
![Collection variables](./Assets/collection_variables.png "Collection variables")




## Running

There are two options to run these requests, either individually or as a collection

### Individual Requests Run

to run an individual request, choose the request from the left hand menu , then press Send to run request.

![run request](./Assets/run_request.png "run request")

### Collection Run

it is possible to run all requests in order, double click on the collection name and choose run:

![run collection](./Assets/run_collection.png "run collection")

a new *Runner* tab will appear:

![runner tab](./Assets/runner_tab.png "runner tab")

this will show all the test results in Postman and will show in the console the summary of information from VirusTotal

![run results](./Assets/run_results.png "run results")


## Closing

this is a quick demo  to highlight how we can use the power of APIs to automate security processes.

as always, PR welcomed.