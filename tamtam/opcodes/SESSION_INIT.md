# SESSION_INIT (6)
Данный опкод отправляется клиентом сразу после подключения к серверу. Содержит данные о приложении - версию приложения, ОС устройства, язык, часовой пояс, userAgent и др.

Сервер отвечает тем же опкодом. (TODO: описать информацию в полезной нагрузке)

Пример запроса:
```json
{
  "ver": 10,
  "cmd": 0,
  "seq": 1,
  "opcode": 6,
  "payload": {
    "userAgent": {
      "deviceType": "WEB",
      "appVersion": "4.12.8",
      "osVersion": "Windows",
      "locale": "ru",
      "deviceLocale": "ru",
      "deviceName": "Chrome",
      "screen": "1024x768 2.0x",
      "headerUserAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)",
      "timezone": "UTC+3"
    },
    "deviceId": "0000000000000000000"
  }
}
```

Пример ответа:
```json
{
  "ver": 10,
  "cmd": 1,
  "seq": 1,
  "opcode": 6,
  "payload": {
    "proxy": "msgproxy.okcdn.ru",
    "logs-enabled": false,
    "proxy-domains": [
      "okcdn.ru",
      "mycdn.me",
      "ok.ru",
      "odnoklassniki.ru",
      "odkl.ru",
      "vk.com",
      "userapi.com",
      "vkuser.net",
      "vkusercdn.ru"
    ],
    "location": "RU",
    "libh-enabled": true
  }
}
```