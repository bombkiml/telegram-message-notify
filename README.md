# Telegram-notify

This package for sending telegram messages notify

## Usage

```js
  const Telegram = require("telegram-notify");
  
  let notify = new Telegram({
    token: "yourTokenString",
    chatId: "yourChatId",
    parse_mode: "html",
  });

  await notify.send("<b>Hello</b> world");
```

## Installation

To use the library, install it through [npm](https://npmjs.com)

```shell
npm install --save telegram-notify
```

## Config

- `token` - Your telegram bot token, create bot: https://t.me/BotFather
- `chatId` - Telegram chat id for notify, get the id: https://t.me/get_id_bot
- `parse_mode` - The Bot API supports basic formatting for messages: https://core.telegram.org/bots/api#formatting-options
- `proxy` - Telegram proxy string [optional], e.q. http://login:password@ip:port
- `maxErrors` - Max attempts to send a telegram message (default:5)

## API

- `send` - Send a telegram message
