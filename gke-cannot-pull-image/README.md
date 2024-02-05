Necessary variables:

```
$PROJECT_ID: This is where to create the Cloud Build resource. This is also the project that has the GKE cluster.
$_CLUSTER_REGION: This is the region of the cluster.
$_CLUSTER_NAME: This is the name of the cluster.
$_IMAGE: This is the image that you're trying to use within the GKE deployment, but don't have access to.
```

To submit this build run the command:

```
gcloud builds submit \
 --project $PROJECT_ID \
 --substitutions=_CLUSTER_REGION=$_CLUSTER_REGION,_CLUSTER_NAME=$_CLUSTER_NAME,_IMAGE=$_IMAGE
```
