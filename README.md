# BanHammer bot

## Features
1. Spam removing
2. "Joined" message removing
3. Global user management

## Spam removing
Bot provides automatic spam detection. Every message is scanned and evaluated. If it reaches certain score of spamness, bot deletes such a message and kick its author out of the chat group. In addition to that: 
* bot kicks the author out of all other groups where the bot is added
* bot puts the author on a blacklist, preventing the author joing any group where the bot is added

Every positive hit of spamness is reported in an admin chat group.
