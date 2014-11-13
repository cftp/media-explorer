Media Explorer
==============
Media Explorer gives you the ability to insert content from social media
services in your posts.

Setup
-----
In order to get this working in your wordpress installation, you have to follow
the next steps:

* Clone this repo in the plugins folder of your WordPress install with `git
clone https://github.com/Automattic/media-explorer.git`.
* Get your credentials for [Twitter](http://dev.twitter.com) and 
[YouTube](https://developers.google.com/youtube/v3/).
* Write your credentials in [mexp-creds.php](https://github.com/Automattic/media-explorer/blob/master/mexp-creds.php)
* Activate the plugin.
* Enjoy!

## Set up Twitter

You will need to create a Twitter app in order to embed tweets using Media Explorer. Here's how:

1. Go to https://apps.twitter.com/
1. Log in with your Twitter account
1. Click on "Create New App"
1. Name your app and fill out a description and the URL
1. Leave "Callback URL" blank
1. Click the button to create your app
1. Once created, click on the "Keys and Access Tokens" tab
1. Copy the "Consumer Key (API Key)" and "Consumer Secret (API Secret)" somewhere
1. Under "Your Access Token" click on the "Create my access token" button
1. Copy the "Access Token" and "Access Token Secret" somewhere
1. Paste these details into the `mexp_twitter_credentials_callback` function in `mexp-credits.php`

## Set up YouTube

You will need to create a Google Code project in order to use Media Explorer with YouTube. Here's how:

1. Go to https://console.developers.google.com/
1. Sign in with a Tab-connected Google account
1. Click on the button to create a project
1. Give it a simple name and click Create
1. Once created, click on "APIs and Auth" in the left hand menu and then "APIs"
1. Scroll down to "YouTube Data API v3" and click the "off" button to the right – this will turn the API on
1. Click on Credentials in the lef-hand menu
1. Under "Public API Access" click "Create new key"
1. Choose "Browser Key" in the prompt
1. Leave the next box blank, clicking Create
1. Copy the API key given and paste it into the `mexp_youtube_developer_key_callback` function in `mexp-credits.php 

## Set up Instragram

You will need to create an Instragram "client" to use Instagram in Media Explorer. Here's how:

1. Go to http://instagram.com/developer
1. Sign in with a Tab-connected account
1. Click "Register your application"
1. Click the green "Register a new client" button
1. Fill in all the required fields. For "Website" and "Oauth redirect URL" enter http://tab.co.uk
1. Paste the Client ID and Client Secret into the `mexp_instagram_credentials_callback` function in `mexp-credits.php`