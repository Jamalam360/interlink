# Interlink
Discord chat bridge (and more) for the ModFest event

## Configuration
When you run the server for the first time the mod will generate a config file `config/modfest.json`.
You can change this file while the server is running and run `/modfest reload` to reload the file.

| Key                 | Description                                          | Example                                                                          |
|---------------------|------------------------------------------------------|----------------------------------------------------------------------------------|
| server.name         | The name used for system webhook logging.            | ModFest 1.16                                                                     |
| server.icon         | URL of a .png image used for system webhook logging. | https://raw.githubusercontent.com/ModFest/modfest.github.io/master/1.16/icon.png |
| discord.webhook     | Discord webhook URL used for logging.                | N/A                                                                              |
| discord.channel     | Channel id that will be linked with the server.      | 730927965462069309                                                               |
| discord.token       | The token for the Discord bot.                       | N/A                                                                              |
| discord.mirrorDeath | If `true`, death messages will be sent to Discord.   | false                                                                            |
| crashes.uploadToHastebin | If `true`, crash reports will be submitted to public paste site [Hastebin](https://hastebin.com/about.md), and the webhook will share a link to it. | true |  

Example config file.
```json
{
  "server": {
    "name": "ModFest 1.16",
    "icon": "https://raw.githubusercontent.com/ModFest/modfest.github.io/master/1.16/icon.png"
  },
  "discord": {
    "webhook": "",
    "channel": "719069949267542056",
    "token": "",
	"mirrorDeath": true
  },
  "crashes": {
	"uploadToHastebin": true
  }
}
```