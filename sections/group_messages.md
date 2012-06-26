GroupMessages
===========

GET GroupMessages
-----------------

`GET /groups/(your-group-id)/group_messages.json` will return all GroupMessages in your Group.

```shell
curl -H 'Authorization: OAuth Add-Your-OAuth2-Token-Here' http://handpick.me/api/v1/groups/(your-group-id-here)/groups_messages.json
```

**Response:**

```json
[{"_id":"4faf2783e5a910000500000b","already_sent":false,"created_at":"2012-05-13T03:16:19+00:00","desc":"using god with resque","desc_md":"\nusing god with resque\n\n","group_id":"4f995520b1ec08000800000a","link":"http://thomasmango.com/2010/05/27/resque-in-production/","message_id":"4faf2783e5a910000500000a","title":"Resque in Production by Thomas Mango","updated_at":"2012-05-13T03:16:19+00:00"}, ...]
```

Update GroupMessage
-------------------

`POST /group_messages/(your-group-message-id).json` will update an existing GroupMessage.

```shell
curl -X POST -H 'Authorization: OAuth Add-Your-OAuth2-Token-Here' -d "title=your-title&link=your-link&desc_md=your-desc-in-markdown" http://handpick.me/api/v1/groups_messages/(your-group-message-id).json
```

This will return a `201 Created`.