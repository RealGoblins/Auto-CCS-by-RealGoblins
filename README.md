# Download
## [Click to get download link](https://sub2unlock.com/JmCT5)
<br><br/>
## VPS files (optional)
1. Download: https://mega.nz/file/JU4jXY6L#_vvkdcRsyxkebC-b0GPbFJiwe41Gz75ke2N-rYQ8XDA
2. Right click -> Extract files
3. Move (drag-drop) `Auto-CCS by RealGoblins.exe` to `VPS_files`

Only if you're running the application on a *VPS/VDS/RDP* you will need additional \*.dll files.
Download the following files and place them **in the same directory as the app**.
This is a Mesa3D software renderer which you'll need if you don't have a GPU.

## VC Redist x64 (optional)
If the app doesn't start, or gives errors such as: mcsv140.dll not found, download and install the following. Note: Only do this if you have already installed the VPS files.
https://aka.ms/vs/17/release/vc_redist.x64.exe

## Pricing

1 DL per bot (monthly)
1 license = 1 bot

|   Bot count   | Gems profit per 30 days | Seed profit per 30 days | DL profit per 30 days (200k gems/DL & 50 seeds/WL) |
| ------------- | ----------------------- | ----------------------- | -------------------------------------------------- | 
| 5             | 39 600 000              | 216 000                 | 241                                                | 
| 15            | 118 800 000             | 648 000                 | 724                                                |
| 50            | 396 000 000             | 2 160 000               | 2 412                                              |

# Tutorials

## Configs
### Socks5 proxy config
note: your proxies must support the UDP protocol. Ask your provider before buying to be sure.
The proxy config is imported from the *Socks5 Proxy* tab in the application

Format:
```
{IP}:{Port}:{Username (optional)}:{Password (optional)}
```

Example: 

```proxy.proxycfg```

```
194.114.5.204:1080:root:rgpw
204.149.2.121:10200
```

### Bot list config
The bot list is imported from left section of the application using the top-left import button.

Format:
```
{GrowID}:{Password}:{farm config (optional)}:{RID for guest logjn (optional)}:{hash for guest logjn (optional)}
```

Example: 

```All bots.botfcfg```

```
AzureBrave47365:YO0C7tdTeR#:bot1.farmcfg
BananaZero43047:eXgl6pynLg#:bot2.farmcfg
BraveFire45181:lrLbHGc5vm#:bot3.farmcfg
DuckGrip80129:Xg3YjIQeI3#:bot4.farmcfg
LiteLuck19932:UyhhLYtAh9#:bot5.farmcfg
TinyBrave14332:7ObO8XpkHb#:bot6.farmcfg
```

### Farm config
This config is unique to each bot and contains the bot settings, including the world list and storage world name. It can be imported by selecting a bot in the left bot list in the application and clicking *import* in the *Rotation*` tab. The config will be auto-imported if it is included in the [Bot list config](#bot-list-config). All settings are configurable from the application too.

Format:
```js
{
    "autoBan": false, // true or false. This will auto-ban if someone joins the farm. (Only works on wl-farms)
    "autoBanIgnore": [], // ['Growid1' , 'player2']. Users to ignore when using the auto-ban feature.
    "autoBuyFromStore": true, // true or false. This will auto-buy from the store and drop to the storage.
    "autoBuyItem": "world_lock_10_pack", // <the item name in the gt store>. This item will be bought using the earned gems and will be dropped to the storage
    "autoBuyItemAmount": 1, // 1 or 2 or more. This is the amount of the *autoBuyItem* that will be bought at once.
    "autoTrash": true, // true or false. This decides whether the bot will auto trash farming drops, such as earth or wind essence
    "autoBuyClothes": true, // true or false. This decides whether the bot will auto buy 1 rare clothes pack (500 gems), in order to prevent getting "detected"
    "storageWorldName": "YOURSTORAGEWORLDHERE", // <Your storage>.The bot will drop the profit here (seeds + store items). The storage MUST be made of display boxes.
    "webhookBots": "", // <WEBHOOK FOR BOT STATUS>. This is optional. A summary for the progress of all bots will be shown here.
    "webhookEvents": "", // <WEBHOOK FOR BOT EVENTS>. This is optional. Bot events, such as disconnections and profit drops will be logged here.
    "itemWhitelist": [], // Optional. These itemIDs will not be trashed, and will be dropped to the storage.
    "switchAccountAfterDelay": true, // true or false. This will switch to a new account after a specified uptime. It will loop forever.
    "switchAccountDelayMinutes": 180, // a number specifing minutes before switching to a new account from the backupAccounts list.
    "switchAccountWhenBanned": true, // true or false. This will switch to a backup account when the current one is suspended.
    "backupAccounts": [ // This is optional. Backup accounts will be used when an account is suspended or for switching after a specified uptime.
        "testacc1:password",
        "testacc2:password"
    ],
    "worlds": [ // World|ID
        "testworld1|id", 
        "testworld2|id",
        "testworld3|id"
    ]
}
```

Example:

```bot1.farmcfg```

```json
{
    "autoBan": false,
    "autoBanIgnore": [],
    "autoBuyFromStore": true,
    "autoBuyItem": "world_lock_10_pack",
    "autoBuyItemAmount": 1,
    "autoTrash": true,
    "autoBuyClothes": true,
    "storageWorldName": "hqks71axd3blqnxo3m9",
    "webhookBots": "https://discord.com/api/webhooks/1143939598605783012/3C16CrHN3bnx-j8In7X0FskxsvABg6lmqpd5K9ev4QvwX9WAjHQFrxlR5eSRkNTuzOw3Z",
    "webhookEvents": "",
    "itemWhitelist": [1828, 4288], 
    "switchAccountAfterDelay": true, 
    "switchAccountDelayMinutes": 180, 
    "switchAccountWhenBanned": true,
    "backupAccounts": [ 
        "jxeutb284asf:goblins123",
        "ino3nz92nsldx:goblins123"
    ],
    "worlds": [
        "2JWCWWHVJJQMYVH5|RGFRM23",
        "5VJKKSM9ULC3OJIM|RGFRM23",
        "FQ55BAZGX8QRR4YS|RGFRM23",
        "HUFXGFUAC61TT1NH|RGFRM23",
        "9HTBVYSFZCGQNCKE|RGFRM23",
        "MWG4NCGJFJJ4JXPQ|RGFRM23",
        "8FRJVJ3UGFRVDAZM|RGFRM23"
    ]
}
```
## What is a Socks5 proxy?
A proxy or proxy server is a computer that sits between you and the server. The network data will be sent from your computer and  to the proxy server and then to the actual destination. The target (actual destination) will not know that you sent the data, it only knows that it was sent from the proxy server. 
Your IP is `X` and you have three proxy servers with the IPs `A`, `B` and `C`. The target server is `Y`.
Without these proxies, the target server will know that you are `X`. But if you use proxies, the server won't know that you are `X`, but that you are `A`, `B` and `C`. In this way, you will be able to use three IPs at once.

To use someone else's IP, you must run a proxy server on a computer on that IP. You then input the Socks5 proxy server `IP:Port`. Such as "192.168.1.1:1080". The proxy **must support UDP** to be compatible.

## How do I get Socks5 Proxies?
You either set up your own proxy servers or you buy proxies. If you buy proxies, you must make sure they support the UDP protocol (the easiest way it to send an email to the company selling the proxies).
To set up a proxy server, you can download a proxy server software and run it on VPS machines or your own virtual machines (which run a VPN to get a new IP). Read the following tutorial.

## Convert rdp to socks5 server
1. **Disable the firewall** 

    Most large VPS providers have this feature in their web panel. On Windows - you can disable the Windows firewall

    <ins>Windows 10, 8, 7:</ins>
    * Go to Control Panel > System and Security > Windows Firewall > Turn Windows Firewall on or off.
    * Click Turn off Windows Firewall in **both sections** and then select OK.
    
2. **Install the socks5 server software**

    Note that some large providers, such as azure and digitalocean, are IP blocked by the GT servers and you can't set them up as socks5 servers

    <ins>Windows:</ins>
    * Download and install: https://update.youngzsoft.com/ccproxy/update/ccproxysetup.exe
    * launch the new ccproxy app. The default socks5 port is 1080
    * (optional) create a username/password in the accounts tab

  
