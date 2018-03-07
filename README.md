= GCP Sample Projects for Autocomplete

== Create a project.

gcloud projects create myproject
gcloud config set project myproject

== Change the links

```
find . -type f -exec sed -i "s/nameofmyproject/nameofyourproject/g" {} \;
```
== Deploy the apps

Deploy the apps in :
gcp/appengine/default
gcp/appengine/autocomplete/appengine

```
gcloud deploy ...
```

The app works but no data ...

== Put the data in a bucket

So put the json.gz files in the bucket :
{{bucketname}}/bestbuy/*.json.gz

Run the scripts in :

gcp/tools/post
gcp/tools/publish

The app shoud work :)

