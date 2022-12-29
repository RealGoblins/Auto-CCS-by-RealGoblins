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

  
