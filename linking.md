# Linking/Whitelisting

The mod supports custom whitelisting via discord.

## Linking Process
By default, `linking.enableLinking` is set to true. When enabled, unlinked players attempting to join the server receive a unique code. They must use this code with the `/link code:<code>` command in Discord to connect their accounts and gain server access.

## Configuration Options
- `linking.requiredRoles`: Set Discord role IDs required for linking permissions
- `linking.joinRoles`: Assign specific Discord roles upon successful Minecraft login
- `linking.renameOnJoin`: Optionally rename Discord users to match their Minecraft usernames (default: true)
- `linking.linkCodeExpireMinutes`: Adjust link code expiration time (default: 10 min)
- `linking.disallowTimeoutMembersToJoin`: Prevent Discord-timed-out members from joining the Minecraft server (default: true)
- `linking.unlinkOnLeave`: Automatically unlink and kick players who leave the Discord server (default: true)

## Alt Account Management
The mod supports linking alternative accounts:
- `linking.maxAlts`: Set a limit on the number of alt accounts per user (default is 1)
- Main account unlink triggers alt account unlink
- Timeouts and role changes affect all linked accounts
