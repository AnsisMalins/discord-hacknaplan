# discord-hacknplan
A Discord bot that responds to mentions of Hacknplan tasks with embeds thereof

To load and run the pyproj, you need to create a file called secrets.txt and fill it with your secrets.
```
--discord-token
asdfgh
--hacknplan-api-key
asdfgh
--hacknplan-project-id
1234
```
To install the bot in production, clone the repository and create a systemd unit file like this one.
```Ini
[Unit]
Description=https://github.com/AnsisMalins/discord-hacknplan
After=network.target

[Service]
ExecStart=/usr/bin/python3 /root/discord-hacknplan/discord_hacknplan.py --discord-token asdfgh --hacknplan-api-key asdfgh --hacknplan-project-id 1234

[Install]
WantedBy=default.target
```
