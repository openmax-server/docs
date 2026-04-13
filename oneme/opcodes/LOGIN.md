# LOGIN (19)
Этот опкод входит в процедуру входа MAX.

Пример ответа сервера:
```json
{
  "ver": 11,
  "cmd": 1,
  "seq": 9,
  "opcode": 19,
  "payload": {
    "profile": {
      "profileOptions": [],
      "contact": {
        "registrationTime": 1776087256000,
        "accountStatus": 0,
        "country": "",
        "baseUrl": "https://i.oneme.ru/i?r=??",
        "names": [
          {
            "name": "Vladimir",
            "firstName": "V",
            "lastName": "Putin",
            "type": "ONEME"
          }
        ],
        "phone": 70000000000,
        "options": [
          "TT",
          "ONEME"
        ],
        "photoId": 1636451375,
        "updateTime": 1776087256000,
        "id": 1,
        "baseRawUrl": "https://i.oneme.ru/i?r=??"
      }
    },
    "chats": [
      {
        "owner": 1,
        "joinTime": 1,
        "created": 1,
        "lastMessage": {
          "sender": 1,
          "id": "36123467233",
          "time": 1776087256000,
          "text": "Ты кто такой",
          "type": "USER",
          "cid": 0,
          "attaches": []
        },
        "type": "DIALOG",
        "lastFireDelayedErrorTime": 0,
        "lastDelayedUpdateTime": 0,
        "prevMessageId": "345346571",
        "modified": 1776087256000,
        "lastEventTime": 1776087256000,
        "id": 2,
        "status": "ACTIVE",
        "participants": {
          "1": 1776087256000,
          "2": 1776087256000
        },
        "cid": 1
      }
    ],
    "messages": {},
    "time": 1776087256000,
    "presence": {},
    "config": {
      "chats": {},
      "server": {},
      "user": {
        "CHATS_PUSH_NOTIFICATION": "ON",
        "PUSH_DETAILS": true,
        "PUSH_SOUND": "oki.aiff",
        "INACTIVE_TTL": "6M",
        "SHOW_READ_MARK": true,
        "AUDIO_TRANSCRIPTION_ENABLED": true,
        "SEARCH_BY_PHONE": "CONTACTS",
        "INCOMING_CALL": "CONTACTS",
        "DOUBLE_TAP_REACTION_DISABLED": false,
        "SAFE_MODE_NO_PIN": true,
        "CHATS_PUSH_SOUND": "oki.aiff",
        "DOUBLE_TAP_REACTION_VALUE": null,
        "FAMILY_PROTECTION": "OFF",
        "HIDDEN": true,
        "CHATS_INVITE": "CONTACTS",
        "PUSH_NEW_CONTACTS": true,
        "UNSAFE_FILES": true,
        "DONT_DISTURB_UNTIL": 0,
        "ALT_KEYBOARD": false,
        "CONTENT_LEVEL_ACCESS": true,
        "STICKERS_SUGGEST": "ON",
        "SAFE_MODE": true,
        "M_CALL_PUSH_NOTIFICATION": "ON"
      },
      "hash": "",
      "experiments": {
        "keep-background-socket": "{\"bg_interval_minutes\":10,\"suggestion_interval_minutes\":4320,\"fg_interval_seconds\":15}",
        "app.ab.test.exp": false,
        "calls-android-early-set-offer": false
      }
    },
    "contacts": [],
    "token": ""
  }
}
```

Здесь названия объектов говорят сами за себя:
- profile - наш профиль
- chats - наши чаты
- contacts - наши контакты
- config - конфиг сервера и остальное