Messages
========

Get Messages
------------

`GET /messages.json` will return all your Messages.

```shell
curl -H 'Authorization: OAuth Add-Your-OAuth2-Token-Here' http://handpick.me/api/v1/messages.json
```

**Response**: 

```json
{"_id":"4fa2e681b37e18000500004a","created_at":"2012-05-03T20:11:45+00:00","desc":"<p>What a story, the guy who started MacRuby did it while working for Apple. When it finally has gotten mature, he left Apple to start his own company to release this.</p><p>I think it's <b></b>gonna be a big hit! Feel like shelling out $150 (limited time offer) to get this.</p><p>Yes. I think I should be getting it.</p>","desc_md":null,"link":"http://www.rubymotion.com/","title":"RubyMotion - Ruby for iOS","updated_at":"2012-05-03T20:33:45+00:00","user_id":"4f812fd28b6684000a000001"}
```

Create Message
--------------

`POST /messages.json` will create a new Message.

```shell
curl -X POST -H 'Authorization: OAuth Add-Your-OAuth2-Token-Here' -d "title=your-title&link=your-link&desc_md=your-desc-in-markdown" http://handpick.me/api/v1/messages.json
```

This will return a `201 Created`.

Get Message
-----------

`GET /messages/(your-message-id).json` will return a specific Message.

```shell
curl -H 'Authorization: OAuth Add-Your-OAuth2-Token-Here' http://handpick.me/api/v1/messages/(your-message-id).json
```

**Response**: 

```json
{"_id":"4fa2e681b37e18000500004a","created_at":"2012-05-03T20:11:45+00:00","desc":"<p>What a story, the guy who started MacRuby did it while working for Apple. When it finally has gotten mature, he left Apple to start his own company to release this.</p><p>I think it's <b></b>gonna be a big hit! Feel like shelling out $150 (limited time offer) to get this.</p><p>Yes. I think I should be getting it.</p>","desc_md":null,"link":"http://www.rubymotion.com/","title":"RubyMotion - Ruby for iOS","updated_at":"2012-05-03T20:33:45+00:00","user_id":"4f812fd28b6684000a000001"}
```

Update Message
-----------

`POST /messages/(your-message-id).json` will return a specific Message.

```shell
curl -X POST -H 'Authorization: OAuth Add-Your-OAuth2-Token-Here' -d "title=your-title&link=your-link&desc_md=your-desc-in-markdown" http://handpick.me/api/v1/messages/(your-message-id).json
```

This will return a `200 Success`.
