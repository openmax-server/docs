# MSG_SEND (64)
Клиент использует этот опкод для отправки сообщений.

Пример запроса:
```json
{
  "ver": 10,
  "cmd": 0,
  "seq": 23,
  "opcode": 64,
  "payload": {
    "chatId": 1,
    "message": {
      "text": "",
      "cid": 111111111,
      "attachMEL": true,
      "detectShare": false
    },
    "notify": true
  }
}
```

где:
- chatId - айди чата
- message/text - текст сообщения
- message/cid - неизвестно
- message/attachMEL - неизвестно
- notify - отправлять уведомление получателю?

Пример ответа:
```json
{
  "ver": 10,
  "cmd": 1,
  "seq": 23,
  "opcode": 64,
  "payload": {
    "chatId": 1,
    "message": {
      "sender": 7783678345,
      "id": "114168742551563583",
      "time": 1774092904351,
      "text": "123",
      "type": "USER",
      "cid": 111111111,
      "attaches": []
    }
  }
}
```