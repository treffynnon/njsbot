A demo Node.js Google Talk Bot
==================
The bot is documented at [njsbot.simonholywell.com](http://njsbot.simonholywell.com "njsbot.simonholywell.com")

Dependencies
------------------
You need a nodester based hosting account such as [cloudno.de](http://cloudno.de "cloudno.de") and the following Node packages:

	npm install node-xmpp request express jade nodester-api
	npm install cloudnode-cli g

To set the bot's password you will need to hit the following URL on your app after it has restarted.

	http://appname.cloudno.de/setup-bot/<hosting service username>/<hosting service password>/<Google Account Password>
