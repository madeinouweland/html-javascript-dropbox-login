# HTML/Javascript Dropbox login/authenticate example

This repo authenticates an App with your Dropbox account and retrieves files from it.

## Flow

![flow](https://github.com/madeinouweland/html-javascript-dropbox-login/blob/master/flow.jpg | width=400)

## Create a dropbox app

On [https://www.dropbox.com/developers/apps](https://www.dropbox.com/developers/apps) you can create an app. When your users use your web app, they will allow access to their dropbox account. When they do, a folder with the app name is created in their dropbox (in the Apps folder) and can now be used by the web app.

## Use Client token

After creating an app, you see an App Key that you fill in in `requestaccess.html` here:
```
var dbx = new Dropbox.Dropbox({ clientId: 'xxxxxxxxx' });
```

## Revoke access

Dropbox users can [revoke access](https://www.dropbox.com/account/connected_apps) from apps

## Start a webserver on mac

Did you know your mac has python installed?
Did you know you can start a webserver serving the current folder with it?

- Open a terminal
- Go to a directory
- Type: `python -m SimpleHTTPServer 8080`
- Browse to [http://127.0.0.1:8080](http://127.0.0.1:8080)
