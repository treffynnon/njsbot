A demo Node.js Google Talk Bot
==================
The bot is documented at [njsbot.simonholywell.com](http://njsbot.simonholywell.com "njsbot.simonholywell.com").

Released under a [BSD license](http://en.wikipedia.org/wiki/BSD_licenses).

Dependencies
------------------
You need a nodester based hosting account such as [cloudno.de](http://cloudno.de "cloudno.de") and the following Node packages:

	npm install node-xmpp request express jade nodester-api
	npm install cloudnode-cli g

To set the bot's password you will need to issue the following curl request and restart your application.

    curl -k -X PUT -u "<cloudno.de username>:<cloudno.de api key/password>" -d "appname=<cloudno.de app name>&key=bot_password&value=<Google Account Password>" https://api.cloudno.de/env
