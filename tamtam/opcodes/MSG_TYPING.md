# MSG_TYPING (65)
Клиент использует этот опкод для отправки индикатора печатания.

Пример запроса:
```json
{
  "ver": 10,
  "cmd": 0,
  "seq": 70,
  "opcode": 65,
  "payload": {
    "chatId": 1,
    "type": "TEXT"
  }
}
```

где:
- chatId - айди чата
- type - тип индикатора ("TEXT", "AUDIO", "VIDEO")

Пример ответа:
```json
{
  "ver": 10,
  "cmd": 1,
  "seq": 70,
  "opcode": 65,
  "payload": null
}
```