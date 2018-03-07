GCP Sample Projects for Autocomplete
========

--- Create a project.
gcloud projects create myproject
gcloud config set project myproject

find . -type f -exec sed -i "s/nameofmyproject/nameofyourproject/g" {} \;

Deploy the apps in :
gcp/appengine/default
gcp/appengine/autocomplete/appengine

The app works but no data ...
So put the json.gz files in the bucket :
{{bucketname}}/bestbuy/*.json.gz

Run the scripts in :

gcp/tools/post
gcp/tools/publish

The app shoud work :)

