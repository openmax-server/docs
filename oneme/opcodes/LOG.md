# LOG (5)
С помощью этого опкода клиент отправляет логи на сервер.

Примеры логов:
```json
{
  "ver": 11,
  "cmd": 0,
  "seq": 2,
  "opcode": 5,
  "payload": {
    "events": [
      {
        "type": "NAV",
        "userId": -1,
        "time": 1,
        "sessionId": 1,
        "event": "COLD_START",
        "params": {
          "action_id": 1,
          "screen_to": 49
        }
      },
      {
        "event": "LOG",
        "type": "AUTH_QR",
        "time": 1,
        "userId": -1,
        "sessionId": 1,
        "params": {
          "qr_ts_ms": 1,
          "action": "web_qr_view",
          "platform": "web",
          "device_id": "",
          "action_id": 1
        }
      },
      {
        "type": "NAV",
        "userId": -1,
        "time": 1,
        "sessionId": 1,
        "event": "GO",
        "params": {
          "action_id": 2,
          "screen_to": 1,
          "screen_from": 49,
          "prev_time": 1
        }
      }
    ]
  }
}
```
