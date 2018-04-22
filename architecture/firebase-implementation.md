# Firebase implementation

## Expo Version

In expo version of Arivaa Basic Firebase, we have used web SDK since expo does not support firebase native SDKs for ios and android.

**Purpose of creating a expo version :**

Many a times, we don't need all the firebase features but only need it as a database and for authentication purposes. Normally Expo does not support Phone, Github and Twitter Authentications by default which we feel might be integral for some applications. Expo version is intended to fully support integration with firebase as a database and support all types of authentication provided by firebase. Expo version does not aim at supporting native features like AdMob, Analytics etc.

**Main Challenges and how we tackled it.**

Phone,Twitter and Github Authentication was not initially supported because of the below reasons :

1. Phone authentication over web requires Recaptcha authentication which is not supported over native platforms, So we had to support it via a webview. 
2. Twitter and Github authentication was not supported since it requires  callback over web. So again webview comes to the solution.

We have tried to optimize the webview experience for above challenges by providing responsive recaptcha implementation and a google UI for handling loading state while webview is processing the request.

However supporting the above features requires you to host a simple webpage\(which does not include any javascript or any risk\) over internet.

