# BanHammer bot

## Features
1. Spam removing
2. "Joined" message removing
3. Global user management
   * Banning user
   * Unbanning user
   * Blacklisting user
   * Whitelisting user

## Spam removing
Bot provides automatic spam detection. Every message is scanned and evaluated. If it reaches certain score of spamness, bot deletes such a message and kick its author out of the chat group. In addition to that: 
* bot kicks the author out of all other groups where the bot is added
* bot puts the author on a blacklist, preventing the author joing any group where the bot is added

Every positive hit of spamness is reported in an admin chat group with a brief description. This gives other admins oportunity to monitor bot's actions. If a positive hit is evaluated as false positive by (human) admin, he can then command the bot to remove the author from a blacklist and unban him in all groups. However, the author himself must join all the chats again.
