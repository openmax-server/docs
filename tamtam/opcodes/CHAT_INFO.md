# CHAT_INFO (48)
Клиент использует данный опкод для запроса информации о чатах.

Пример запроса:
```json
{
  "ver": 10,
  "cmd": 0,
  "seq": 163,
  "opcode": 48,
  "payload": {
    "chatIds": [
      -1
    ]
  }
}
```

где:
- chatIds - массив айди чатов, о которых запрашивается информация

Пример ответа:
```json
{
  "ver": 10,
  "cmd": 1,
  "seq": 14,
  "opcode": 48,
  "payload": {
    "chats": [
      {
        "owner": 3441,
        "joinTime": 1,
        "created": 1,
        "lastMessage": {
          "sender": 3441,
          "elements": [
            {
              "length": 2,
              "entityId": 45,
              "attributes": {
                "animojiSetId": "1",
                "animojiLottieUrl": "https://st.okcdn.ru/static/messages/2023-08-14animoji/54.json"
              },
              "type": "ANIMOJI"
            }
          ],
          "id": "673667",
          "time": 1788275024022,
          "text": "👋",
          "type": "USER",
          "cid": 673667,
          "attaches": []
        },
        "type": "DIALOG",
        "lastFireDelayedErrorTime": 0,
        "lastDelayedUpdateTime": 0,
        "newMessages": 2,
        "lastEventTime": 1788292141357,
        "id": 386502760581,
        "status": "ACTIVE",
        "participants": {
          "3441": 1774477691441,
          "3442": 1784330561562
        },
        "cid": 3441
      }
    ]
  }
}
```
