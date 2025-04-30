# How to set up

## 1. Create your bot

1. Go to https://discord.com/developers/applications/ and click "New Application".

2. Choose a name for your bot and upload an App icon (this will be the bot's default avatar).

3. In the left sidebar, click on "Bot".

4. On the right side of the page, click "Add Bot".

The page should now display your newly created bot's information and settings:
![Bot in developer portal](img/image.png)

On this page, enable at least shown intents:
![intents](img/image-1.png)

## 2. Invite your bot

In the category `OAuth2` select `bot` and `applications.commands` in your OAuth2 URL Generator. And select needed permissions or simply administrator. 
![permissions](image.png)
Use the generated URL to invite your bot.

Alternatively you can use following url which has all necessary permissions `https://discord.com/oauth2/authorize?client_id=1<client_id>&permissions=671108096&integration_type=0&scope=bot+applications.commands`. Just replace `<client_id>` with your client id.

## 3. Add mod to your Minecraft server

1. Download the latest version of the mod from Modrinth or GitHub (or alternatively build it yourself if you know how).
2. Place the .jar file in your server's "mods" folder.
3. Start the server (it will crash, generating a config file).

## 4. Set up config

1. Find the config file in `config/discord-js/`.
2. Add your bot token (from the developer portal) to the config.
3. Add your Discord channel ID to the config.

To get a Discord channel ID:
1. Enable Developer Mode in Discord (User Settings > App Settings > Advanced).
2. Right-click on the desired channel and select "Copy ID".

Start your Minecraft server again, and the Discord bot should now be operational.

It is recommended to take your time and explore the wiki and/or the config file to set the mod up to your needs and give all required information for the mod to work without any issues.
