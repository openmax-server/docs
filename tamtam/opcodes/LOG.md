# LOG (5)
С помощью этого опкода клиент отправляет логи на сервер. Логи на основном веб-клиенте отсутствуют (замечены только на тестовом).

Примеры логов:
```json
{
  "ver": 10,
  "cmd": 0,
  "seq": 220,
  "opcode": 5,
  "payload": {
    "events": [
      {
        "type": "NET",
        "event": "CONFIG",
        "params": {
          "respTime": 54,
          "tamTime": 0
        },
        "time": 1774125984963
      },
      {
        "type": "SCREEN",
        "event": "SETTINGS_BLACKLIST",
        "time": 1774125984970
      },
      {
        "type": "SCREEN",
        "event": "SETTINGS",
        "time": 1774125984970
      },
      {
        "type": "NET",
        "event": "CONTACT_LIST",
        "params": {
          "respTime": 73,
          "tamTime": 0
        },
        "time": 1774125985043
      }
    ]
  }
}
```
