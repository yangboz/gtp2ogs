gtp2ogs
=======

This script allows Go bots that support GTP (Go Text Protocol) to communicate
with OGS (Online-Go.com Server)

Installation
============

  1. Use your systems package manager or otherwise install `node.js` from http://nodejs.org/
  2. Run
    ```
    npm install -g gtp2ogs
    ```
  3. Install any missing node.js packages if basic usage below fails, such as:
    ```
    npm install socket.io-client optimist tracer
    ```


Basic usage
===========

```
gtp2ogs --botid <id> --apikey <apikey> <arguments> -- <bot command> <bot arguments>
```

Steps to connect with a bot
=================================
If you have a go bot that can communicate using the Go Text Protocol (GTP)6, you use a tool like gtp2ogs so it can communicate to OGS.

The basics are:

Make an account for the bot on OGS.
Ask a moderator to flag the account as a bot account.
Set the admin in the bot's profile page.
Log in as your normal admin account and visit bot profile to get an API key generated.

Then run your bot using a command line roughly like:

node gtp2ogs.js --username YourBotNameHere --apikey yourkeyhere --debug -- yourbotprogram.exe >> log 2>&1

More advanced command line options are available to gtp2ogs depending on your needs and the bot. Any more command line strings after the name of the bot is passed to the bot itself.

References
=================================

https://forums.online-go.com/t/steps-to-connect-with-a-bot/11234

