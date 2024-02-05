Necessary variables:

```
$PROJECT_ID: This is where to create the Cloud Build resource and Cloud Run resource.
```

To disable the cloud run api:
```
gcloud services disable run.googleapis.com --project $PROJECT_ID --force
```

To submit this build run the command:

```
gcloud builds submit --project $PROJECT_ID
```
