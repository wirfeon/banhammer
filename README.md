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

![joined removed]("banhammer/Screenshot from 2019-02-19 14-27-35.png")

## 3. User management
Bot provides several commands for managing users across all groups where it is added. All these commands has to be run in bot's admin group chat.

### Banning user
An admin must first forward a message of a user who is to be banned. This marks the user for the bot. Admin then reply to this forwarded message with /ban command. Bot puts the author of the message on a blacklist and kicks him from every chat group.

## 4. Bot management
