# Auto-CCS by RealGoblins (5 dls)

## Download
https://github.com/RealGoblins/Auto-CCS-by-RealGoblins/raw/main/Auto-CCS%20by%20RealGoblins.exe 

## VPS files (optional)
Only if you're running the application on a *VPS/VDS/RDP* you will need additional \*.dll files.
Download the following files and place them **in the same directory as the app**.
This is a Mesa3D software renderer which you'll need if you don't have a GPU.
1. Download: https://mega.nz/file/JU4jXY6L#_vvkdcRsyxkebC-b0GPbFJiwe41Gz75ke2N-rYQ8XDA
2. Right click -> Extract files
3. Move (drag-drop) `Auto-CCS by RealGoblins.exe` to `VPS_files`

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
{GrowID}:{Password}:{farm config (optional)}
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

  
