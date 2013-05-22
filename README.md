A demo Node.js Google Talk Bot   [![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](http://flattr.com/thing/1146002/)
==============================
The bot is documented at [njsbot.simonholywell.com](http://njsbot.simonholywell.com "njsbot.simonholywell.com").

Released under a [BSD license](http://en.wikipedia.org/wiki/BSD_licenses).

Google Hangouts
---------------
With the introduction of Google Hangouts and its intended replacement of Google Talk including [phasing out support for XMPP](http://windowspbx.blogspot.co.uk/2013/05/hangouts-wont-hangout-with-other.html) this client is becoming less relevant. It can still be used as a basis for bots communicating over XMPP networks and for those who wish to use Google Talk rather than upgrading to Hangouts.

I can confirm from testing that once a user upgrades to use a Hangouts client (web chat in Gmail, Android client, etc) that the njsbot is no longer visible in their contacts list. According to all the information and documentation I have read this change is unlikely to be reversed or result in eventual support of XMPP wthin Hangouts itself.

If you wish to learn about the new Hangouts API then checkout it's documentation [here](https://developers.google.com/+/hangouts/api/).


Dependencies
------------
You need a nodester based hosting account such as [cloudno.de](http://cloudno.de "cloudno.de") and the following Node packages:

	npm install node-xmpp request express jade

If on cloudno.de then also

	npm install cloudnode-cli g

To set the bot's password you will need to issue the following curl request and restart your application.

    curl -k -X PUT -u "<cloudno.de username>:<cloudno.de api key/password>" -d "appname=<cloudno.de app name>&key=bot_password&value=<Google Account Password>" https://api.cloudno.de/env
