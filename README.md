# Google Cloud Functions Course

## Starting a project
To start a new project in Google Cloud, we can go to the 
[Firebase Console](https://console.firebase.google.com)
or create it from [Google Cloud Platform Console](https://console.cloud.google.com).

## Creating a virtual environment

First we install ` python - virtualenv `
```
pip install virtualenv
```
Then create a virtual environment called 'venv'
```
virtualenv venv
```
And we activate the environment:

```
.\venv\Scripts\activate.ps1
```
We install the requirements:
```
pip install -r .\requirements.txt
```

## Deploying our functions
First, we have to set our project ID with the following 
command:
```
gcloud config set project [YOUR_PROJECT_ID]
```
Then we deploy our function with this command:
```
gcloud functions deploy [FUNCTION_NAME] --runtime python37 --trigger-http
```


