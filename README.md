# role-email-to-telegram

Ansible role for setting up 
[email-to-telegram](https://github.com/ItsNotGoodName/email-to-telegram) on 
Debian 10.

## Variables
```yaml
# API token from BotFather
telegram_token: 12345678

# Matches email's 'to_address' and/or 'from_address' to a chat with chat_id.
# Having no 'to_address' or 'from_address' will allow all emails to that chat.
# (The bot must be part of the chat to be able to send messages)
telegram_transfers:
  - chat_id: -1001111111111
    to_address: channel1@telegram.lan
    from_address: ip-camera@telegram.lan
    disable_text: False
    disable_photo: False
```
