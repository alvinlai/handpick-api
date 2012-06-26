Handpick Developer API
============

The API for Handpick is currently in beta but I'm already using it for the iOS app. I might make mior changes and improvements but I'll try to keep everything as it is.

If you're planning to connect Handpick with your app, let me know!

Join me and other developers at the [Handpick Developer Forum](https://groups.google.com/forum/#!forum/handpick-developers).

You can also personally email me at [al@alvinlai.com](mailto:al@alvinlai.com) if you want early access.

Authentication
--------------

Handpick's API requires OAuth2 authentication. To get started, you'll need to:

- Sign in to your Handpick account
- Register your application to receive your OAuth2 key and secret
- Authenticate and get your OAuth2 Token
- Authorize by adding an `Authorization` header with your `OAuth Add-Your-OAuth2-Token-Here` OAuth2 Token.

Making a request
----------------

Remember to add the `Authorization` header with `OAuth Add-Your-OAuth2-Token-Here`. Here's an example using Curl:

  curl -H 'Authorization: OAuth Add-Your-OAuth2-Token-Here' http://handpick.me/api/v1/groups.json

API Endpoints
-------------

* [Groups]
* [GroupMessages]
* [Messages]

Help improve Handpick's API
---------------------------

Please let me know how I can make the API better. Create Github issues for specific feature requests or for filing a bug. Fork this repository and send a pull request with improvements.

To chat with me and other developers about the API, join the [Handpick Developer Forum](https://groups.google.com/forum/#!forum/handpick-developers).