Groups
======

Get Groups
----------

`GET /groups.json` will return all your Groups you own

```shell
curl -H 'Authorization: OAuth Add-Your-OAuth2-Token-Here' http://handpick.me/api/v1/groups.json
```

**Response:**

```json
[{"_id":"4f995520b1ec08000800000a",
"api_token":"eb1e577997edd0",
"bcc":false,
"clear_stories_after_delivery":false,
"contributable":false,
"created_at":"2012-04-26T07:01:04-07:00",
"email_conclusion":,
"email_delivery_days":"Everyday",
"email_introduction":,
"email_subject":"I've handpicked some interesting links for you today.",
"hidden":false,
"hide_timestamps":false,
"local_delivery_time":"2012-04-26T10:00:00-07:00",
"name":"!!Braindump",
"public":false,
"subscribable":false,
"time_zone":"Pacific Time (US & Canada)",
"updated_at":"2012-05-06T16:23:57-07:00",
"user_id":"4f812fd28b6684000a000001",
"utc_delivery_time":"2012-05-07T00:00:00Z",
"utc_hour":0,
"utc_minute":0}, ...]
```