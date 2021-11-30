# Postman Calls for the EUROPACE APIs

Test calls to the APIs are very helpful to get started quickly. For this we recommend [Postman](https://www.getpostman.com/), which works on Windows, Mac OS and Linux.

## Requirements to call APIs:

1. API access with OAuth client credentials. How to get the client is [described here](https://docs.api.europace.de/baufinanzierung/authentifizierung/#wie-bekomme-ich-einen-client-registriert).
2. at least one [Vorgang](https://docs.api.europace.de/common/glossary) or [Antrag](https://docs.api.europace.de/common/glossary) to read the data.

## Steps to set up Postman
1. Postman [download](https://www.getpostman.com/) and install. There is *no* registration required.

2. click on _Import_ button in the upper left corner, then on _Import from Link_.
![](https://raw.githubusercontent.com/europace/api-schnellstart/master/screen01.png)

3. paste the following link into the textbox: `https://raw.githubusercontent.com/europace/api-sandbox/master/EUROPACE%20API%20Calls.postman_collection.json`.
![](https://raw.githubusercontent.com/europace/api-schnellstart/master/screen02.png)

4. create a new _Environment_ in which several necessary variables must be entered. To do this, click the icon in the upper right corner:
![](https://raw.githubusercontent.com/europace/api-schnellstart/master/screen03.png)

5. give your _Environment_ a name and create the following variables in it:

| Variable Name | Where do I get this? |
| -------------- | ---------------------- |
| PARTNER_ID | See above under "Requirements" |
| CLIENT_ID | See above under "Requirements" |
| CLIENT_SECRET | See above under "Requirements" |

![](https://raw.githubusercontent.com/europace/api-schnellstart/master/screen04.png)

5. after creating the _Environment_, make sure that it is active:
![](https://raw.githubusercontent.com/europace/api-schnellstart/master/screen05.png)


## Try it out
6. click on the call in the new collection in the left column (`Get OAuth Access-Token`).
![](https://raw.githubusercontent.com/europace/api-schnellstart/master/screen06.png)


7. when you click on _send_ you should get an `access_token` back. The request will store the access_token into a global variable named `{{access_token}}` to use the token in further requests. You are now logged in and can use the apis.
![](https://raw.githubusercontent.com/europace/api-schnellstart/master/screen07.png)

8. try out the awsome europace apis