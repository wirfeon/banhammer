# BanHammer bot

## Features
1. Spam removing
2. "Joined" message removing
3. User management
   * Banning user
   * Unbanning user
   * Blacklisting user
   * Whitelisting user
4. Bot management
   
## 1. Spam removing
Bot provides automatic spam detection. Every message is scanned and evaluated. If it reaches certain score of spamness, bot deletes such a message and kick its author out of the chat group. In addition to that: 
* bot kicks the author out of all other groups where the bot is added
* bot puts the author on a blacklist, preventing the author joing any group where the bot is added

Every positive hit is reported in bot's admin chat group with a brief description. This gives other admins oportunity to monitor bot's actions. If a positive hit is evaluated as false positive by (human) admin, he can then command the bot to remove the author from a blacklist and unban him in all groups. However, the author himself must join all the chats again.

## 2. "Joined" message removing
Bot deletes every system message that informs of a user joing a chat group.

![Joined message removed](sc-removed.png)

## 3. User management
Bot provides several commands for managing users across all groups where it is added. All these commands has to be run in bot's admin group chat.

### Banning user
An admin must first forward a message of a user who is to be banned. This marks the user for the bot. Admin then reply to this forwarded message with /ban command. Bot puts the author of the message on a blacklist and kicks him from every chat group.

![User banned](sc-banned.png)

## 4. Bot management
In order to add the bot to a new chat group, one must authorize that chat by executing /enable command. Without authorization the bot will leave the new chat immediately after joining. /enable takes one arugment and that is a chat ID 

[!Chat authorized](sc-enabled.png)

Use /whereami to see where the bot is added

[!Whereami](sc-whereami.png)
