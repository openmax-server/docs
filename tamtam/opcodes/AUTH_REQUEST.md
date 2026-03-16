# AUTH_REQUEST (17)
Клиент использует этот опкод для запроса кода SMS на номер телефона. Это первый опкод в процессе авторизации.

Пример запроса:
```json
{
  "ver": 10,
  "cmd": 0,
  "seq": 4,
  "opcode": 17,
  "payload": {
    "phone": "+70000000000",
    "requestType": "SMS"
  }
}
```

Пример ответа:
```json
{
  "ver": 10,
  "cmd": 1,
  "seq": 4,
  "opcode": 17,
  "payload": {
    "callDelay": 0,
    "codeDelay": 120,
    "codeLength": 6,
    "requestType": "SMS",
    "retries": 5,
    "verifyToken": "A48sRmsCEaqvO3Dd"
  }
}
```

где:
- codeLength - количество символов в коде
- retries - количество допустимых попыток
- verifyToken - токен верификации, понадобится позже
