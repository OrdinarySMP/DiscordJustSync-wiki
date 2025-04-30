# Command logging

Discord-JustSync supports the logging of commands to one or more Discord channels.  \
The main logging channel is defined with `consoleChannel`. All executed commands will be logged to that channel. \
This channel is also used for [executing commands from discord](Execute-commands-on-discord) \
You can toggle the command logging with the `logCommandsInConsole` option. \
It is possible to ignore commands with the `ignoredCommands` option. You can pass multiple commands like this: `ignoredCommands = ["me", "say"]` \
Command blocks can be logged with the `logCommandBlockCommands` option. It is not recommended to enable this as it can hit the rate limit of Discord really fast.


## Log redirect channels
Specific commands can be redirected to a different channel. It is possible to configure multiple redirect channels. \
You can configure them as follows:
```toml
[[commands.logRedirectChannels]]
channel = "1234567890"
redirectPrefixes = ["w ", "msg ", "tell "]
```
Note: The space after the command is required to not match other commands. For example "w" would also match the command `worldborder`.
