# Discord Command Execution

Discord commands can be executed directly through the console channel. This feature is enabled by default and can only be disabled by removing all default commands from the config.

## Setup

1. Use the console channel for command execution (see [command logging](Command-logging)).
2. Send commands with the specified prefix (`commands.commandPrefix`, default=`//`).
3. Default commands: `/kill`, `/kick`, `/ban`, and `/stop`.

## Custom Commands

Add custom commands in the config using this format:


```toml
[[commands.commandList]]
# Name of the command on discord
commandName = "kill"
# Command to run ingame, use Placeholder %args% for args
inGameAction = "kill %args%"
```


The `%args%` placeholder allows passing arguments from Discord to the in-game command. For example, sending `//kill MoFen` on Discord executes the corresponding command on the server.
