# Floodgate Integration


[Floodgate](https://modrinth.com/mod/floodgate) is a mod which you can install alongside [Geyser](https://geysermc.org/) to let players join on Bedrock edition without having a Java account.

If the `maxAlts` option is set at 0 and no alts are allowed these features don't take any effect.

You can restricted players from either linking or joining with mixed account types (meaning java and bedrock). If players are not allowed to link, they will receive the configured response if they already have an account linked and are trying to link an account of different type.
Restricting mixed account types to join will automatically disconnect players with the configured kick message if another one of their linked accounts is online and of different type.

Both of these options can be bypassed with a list of discord roles.


Config snippet:
```toml
[integrations.floodgate]

allowLinkingMixedAccountTypes = true

allowLinkingMixedAccountTypesBypass = ["123456789", "123123"]

linkingMixedAccountTypesDenyMessage = "You are not allowed to mix account types on this server"


allowJoiningMixedAccountTypes = true

allowJoiningMixedAccountTypesBypass = []

joiningMixedAccountTypesKickMessage = "You are not allowed to join with mixed account types at the same time"
```
