# Customizing Messages in Discord: JustSync

Discord: JustSync allows message customization using the [Placeholder API](https://placeholders.pb4.eu/user/text-format/). You can modify text appearance using simple XML tags like color changes (`<blue>text</blue>`), italics (`<i>text</i>`), clickable links (`<url:%link%>text</url>`), and more.

## Customizable Messages

- Chat message: `message.chatMessageFormat`
- Chat message reply: `message.chatMessageFormatReply`
- Link formatting: `message.linkFormat`
- Discord attachments: `messages.attachmentFormat`
- Command logging: `messages.commandExecutedInfoText`
- Join messages: `messages.playerJoinMessage`
- Leave messages: `messages.playerLeaveMessage`
- Advancements: `messages.advancementMessage`
- Server start: `messages.startMessage`
- Server stop: `messages.stopMessage`
- Server count bot status: `messages.onlineCount*`

## Common Placeholders (not by Placeholder API)

- `%user%`: Discord username
- `%msg%`: Message content
- `%userRepliedTo%`: User being replied to
- `%attachments%`: Attached files
- `%link%`: (Attachment) URL
- `%name%`: Attachment name
- `%cmd%`: Executed command

Note: Check the config file for specific placeholder usage and functionality for each message type.

For kick message customization, refer to [kick-message](Kick-messages).
