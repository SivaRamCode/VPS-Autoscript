#### ***About***

This script will install:

Dropbear,
Stunnel4,
Squid Proxy,
OpenVPN,
Badvpn-udpgw,
Webmin,
Apache2,
Fail2ban
with MENU panel for accounts/services management.


Optional: WS+Dropbear, WS+SSL, WS+Ovpn




#### ***Installation***
 
Please install on a fresh deployed Ubuntu 18.04/20.04 or Debian 9/10 to minimize errors.

Installer was tested using AWS Lightsail Instances.

##### Run command:
```bash
rm -f myCode && wget -O vpsphc "https://raw.githubusercontent.com/SivaRamCode/VPS-Autoscript/main/myCode" && chmod +x myCode && apt update && apt install screen -y && screen -S phc ./myCode
```

#### ***Note***
In case you get disconnected during installation, just relogin to your vps and type the command:
```bash
screen -r
```
## Services ##
Dropbear 143

Squid 7799

Stunnel (Dropbear:442 Openvpn-SSL:444)

Openvpn TCP 1194

Openvpn UDP 1196

Webmin 10000

Badvpn-udpgw 7300

Apache2(for ovpn config link) 88


To enable ws for gtm noload run command: startnoload

WS+Dropbear 80

WS+Stunnel 443

WS+Openvpn 99 


#### ***Credits***
All credits goes to the masters of related projects

-[Bon-chan](https://github.com/bonveio)

-[Fast VPN](https://phcorner.net/threads/976085/) for badvpn tutorial

-[N O T E](https://github.com/darkrenz) for websocket
