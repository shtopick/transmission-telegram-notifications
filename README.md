# Bash script that sends a message to the telegram bot after the transmission finishes downloading a torrent.

<b><h2>Instructions:</h2></b>
Put the script in a folder at your choice

Stop tansmission-deamon service

sudo service transmission-daemon stop

Allow the execution of the script

sudo chmod +rx transmission_telegram_notification.sh

Open the transmission-daemon settings file

sudo nano /etc/transmission-daemon/settings.json

Change the following:

 "script-torrent-done-enabled": true,
 "script-torrent-done-filename": "/your/script/path",
Save the changes and start the transmission-daemon service

sudo service transmission-daemon start

Note: Those variables are inherited from Transmission

TR_TIME_LOCALTIME
TR_TORRENT_NAME
