# NOTIF_MESSAGE (128)
Сервер использует этот опкод для оповещения клиента о входящем сообщении.

Пример:
```json
{
  "ver": 10,
  "cmd": 0,
  "seq": 5,
  "opcode": 128,
  "payload": {
    "chatId": 1,
    "message": {
      "sender": 10000,
      "id": "14319216523467",
      "time": 1774477002144,
      "text": "Куку гага",
      "type": "USER",
      "cid": 166277431662,
      "attaches": []
    },
    "ttl": false,
    "prevMessageId": "14319216523466"
  }
}
```

где:
- chatId - айди чата, из которого пришло сообщение
- message/sender - айди отправителя сообщения
- message/id - айди сообщения
- message/text - текст сообщения
- message/cid - ??
- message/attaches - прикреплённые файлы
- ttl - ??
- prevMessageId - предыдущее айди сообщения в чате
