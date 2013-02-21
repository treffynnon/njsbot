A demo Node.js Google Talk Bot   [![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=treffynnon&url=https://github.com/treffynnon/njsbot&title=njsbot&language=&tags=github&category=software)
==============================
The bot is documented at [njsbot.simonholywell.com](http://njsbot.simonholywell.com "njsbot.simonholywell.com").

Released under a [BSD license](http://en.wikipedia.org/wiki/BSD_licenses).

Dependencies
------------
You need a nodester based hosting account such as [cloudno.de](http://cloudno.de "cloudno.de") and the following Node packages:

	npm install node-xmpp request express jade

If on cloudno.de then also

	npm install cloudnode-cli g

To set the bot's password you will need to issue the following curl request and restart your application.

    curl -k -X PUT -u "<cloudno.de username>:<cloudno.de api key/password>" -d "appname=<cloudno.de app name>&key=bot_password&value=<Google Account Password>" https://api.cloudno.de/env
