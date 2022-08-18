gsutil is a tool to access the cloud storage services, is a CLI.

```
gsutil ls # to list the content the content of cloud storage to this project

gsutil mb #Make bucket "gs://{BUCKET-NAME}

gsutil ls {BUCKET-NAME} # shows the content of the bucket

gsutil cp {SOURCE} {DESTINATION} #Copy a file to a another site this is used for example to upload and download files

```

The objects are staticks and if you change the content of a file and you upload it, it will overwrite it