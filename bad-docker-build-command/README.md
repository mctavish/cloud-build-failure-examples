Necessary variables:

```
$PROJECT_ID: This is where to create the Cloud Build resource.
$_TARGET_REPO_TAG: This is the tag that you're trying to tag your image.
```

To submit this build run the command:

```
gcloud builds submit \
 --project $PROJECT_ID \
 --substitutions=_TARGET_REPO_TAG=$_TARGET_REPO_TAG
```
