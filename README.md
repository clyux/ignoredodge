# ignoredodge

A Minecraft Forge 1.8.9 mod that exploits a bug on Hypixel to identify nicked players in pregame.

> [!CAUTION]
> This mod breaks Hypixel's server rules and I cannot guarantee it is undetectable.

[Hypixel's Statement on Automation](https://support.hypixel.net/hc/en-us/articles/6472550754962-Hypixel-Allowed-Modifications)

# How it works

On Hypixel, if you `/ignore add <some player>`, the server can respond in three ways:

<img width="987" height="152" alt="image" src="https://github.com/user-attachments/assets/eb65f7d4-664a-4f25-89bd-7c65d60cb04d" />

<img width="366" height="46" alt="image" src="https://github.com/user-attachments/assets/ba99cc6d-1df7-4e1e-8cca-85e0c27d3652" />

<img width="333" height="50" alt="image" src="https://github.com/user-attachments/assets/5139cbc5-86f5-4e65-bfe1-d189e146fd7c" />

To use this to dodge nicks, running `/ignore add <nick>` means we are looking for the following responses:

`Blocked <nick>.` 

or 

`You've already blocked that player! /block remove <nick> to unblock them!`

These messages are both considered a success, meaning that the nick is in the game with you.

If the player you are trying to dodge unnicks, this bug no longer works.

# Usage

`/ignoredodge` parent command reveals the help menu for the mod.

## Known issues

1. No extra checks for requeue failure
2. Config is not persistent
3. probably a bunch more I forgot about
