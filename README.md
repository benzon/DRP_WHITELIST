# [Beta] DRP_WHITELIST - v1.0
**Version:** 1.0
**Created by:** BenZoN - DanishRP

**Requirements DRP_WHITELIST**

[fivem-mysql-async v3.0.x](https://github.com/brouznouf/fivem-mysql-async)
[Essentialmode](https://essentialmode.com/)

**Note**

This is in BETA, would love some feedback on the system when tested on FiveM Forums

**Description**

This is just another MySQL Whitelist script, but done the way I wanted a whitelist script to work.

Most whitelist scripts I have tried, where either missing the feature to add SteamID’s or License ID’s on the fly, with out having to run a reload command, or restart the script, and you had to convert the SteamID to hex.

And that is why I created this script, it supports adding steam id’s with out having to convert them to hex, and it support’s the usage of license identifier to, the in-game commands are based on essentialmode, but it features rcon commands to, and from what I read they support’s ace permissions, so it can be made a standalone release quite easy.

But I don't got enough experience with ace permissions, I would love to hear more about it, so I can do a 100% standalone release. 

Supports translation - credits: [es_extended](https://github.com/ESX-Org/es_extended)

**Features**
- Supports SteamID64 (steam:*****************)
- Supports License ID (license:**)
- Simple SteamID validation counts numbers after steam: should be 17
- Simple License ID validation counts numbers/letter after license: should be 40
- Supports rcon commands
- Remove SteamID and License ID via rcon and essentialmode command
- You can remove SteamID’s in 64 format or in HEX format!

**Installation DRP_WHITELIST**
- Download - https://github.com/benzon/DRP_WHITELIST/archive/master.zip
- Put it in the `resources` directory
- Add this to your  `server.cfg`:
```
start DRP_WHITELIST
```

Import **whitelist.sql** to your database

**Commands**
- /addwl ID (ex. steam:76561197960287930)
- /removewl ID (ex. steam:76561197960287930 or steam:1100001000056ba)
- rconaddwl ID (ex. license:xxx)
- rconremovewl ID (ex. license:xxx or steam:76561197960287930)

**Credits/Inspiration**
essentialmode - The way there ban system is done where an inspiration to validate the whitelist.
WhiteList DB (Async) 2.0 - Inspiration to add rcon command, sadly this release is out of date and got some bugs.
es_extended - Credits for locale.lua (It's only included in the release to make it more standalone, and not require esx)

## Legal
DRP_WHITELIST - DRP Whitelist

Copyright (C) 2015-2019 BenZoN

This program Is free software: you can redistribute it And/Or modify it under the terms Of the GNU General Public License As published by the Free Software Foundation, either version 3 Of the License, Or (at your option) any later version.

This program Is distributed In the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty Of MERCHANTABILITY Or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License For more details.

You should have received a copy Of the GNU General Public License along with this program. If Not, see  [http://www.gnu.org/licenses/](http://www.gnu.org/licenses/).