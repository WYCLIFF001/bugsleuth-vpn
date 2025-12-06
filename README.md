<p align="center">
<h1 align="center">Auto Script VPN Service Installer</h1>
<h2 align="center">SSH/OpenVPN/XRAY with Telegram Bot Management</h2>
<p align="center">
<img src="https://img.shields.io/badge/Release-v0.1.0-blue.svg">
<img src="https://img.shields.io/badge/Systemd-Required-green.svg">
<img src="https://img.shields.io/badge/License-MIT-yellow.svg">
</p>
</p>

---

<h2 align="center">Supported Linux Distribution</h2>
<p align="center"><img src="https://d33wubrfki0l68.cloudfront.net/5911c43be3b1da526ed609e9c55783d9d0f6b066/9858b/assets/img/debian-ubuntu-hover.png" width="400"></p>
<p align="center">
<img src="https://img.shields.io/static/v1?style=for-the-badge&logo=debian&label=Debian%2010&message=Buster&color=purple">
<img src="https://img.shields.io/static/v1?style=for-the-badge&logo=debian&label=Debian%2011&message=Bullseye&color=purple">
<img src="https://img.shields.io/static/v1?style=for-the-badge&logo=debian&label=Debian%2012&message=Bookworm&color=purple">
</p>
<p align="center">
<img src="https://img.shields.io/static/v1?style=for-the-badge&logo=ubuntu&label=Ubuntu%2020.04&message=Focal&color=red">
<img src="https://img.shields.io/static/v1?style=for-the-badge&logo=ubuntu&label=Ubuntu%2022.04&message=Jammy&color=red">
<img src="https://img.shields.io/static/v1?style=for-the-badge&logo=ubuntu&label=Ubuntu%2024.04&message=Noble&color=red">
</p>

---

<h2 align="center">Network Protocols</h2>
<h2 align="center">

![SSH](https://img.shields.io/badge/SSH-WebSocket-8020f3?style=for-the-badge&logo=Cloudflare&logoColor=white)
![OpenVPN](https://img.shields.io/badge/OpenVPN-TCP/UDP-20f380?style=for-the-badge&logo=Cloudflare&logoColor=white)
![VMESS](https://img.shields.io/badge/XRAY-Vmess-f34b20?style=for-the-badge&logo=Cloudflare&logoColor=white)
![VLESS](https://img.shields.io/badge/XRAY-VLess-f34b20?style=for-the-badge&logo=Cloudflare&logoColor=white)
![TROJAN](https://img.shields.io/badge/XRAY-Trojan-f34b20?style=for-the-badge&logo=Cloudflare&logoColor=white)

</h2>

---

## 📋 Requirements

1. Domain Name
2. Telegram Bot Token (Get from [@BotFather](https://t.me/botfather))
3. VPS with Root Access
4. Systemd Support

---

## ☁️ Cloudflare Settings

**PLEASE CONFIGURE YOUR DOMAIN IN CLOUDFLARE AS BELOW:**

| Setting | Value |
|---------|-------|
| SSL/TLS Encryption Mode | **Full** |
| SSL/TLS Recommender | **OFF** ❌ |
| gRPC | **ON** ✅ |
| WebSocket | **ON** ✅ |
| Always Use HTTPS | **OFF** ❌ |
| Under Attack Mode | **OFF** ❌ |

**DNS Configuration:** Set DNS record to **DNS Only** (Grey Cloud) - Point to your VPS IP

---

## 🚀 Installation

### Debian 10/11/12 (Buster/Bullseye/Bookworm)

**First Time Setup:**
```bash
apt update -y && apt install -y wget curl && apt upgrade -y && apt dist-upgrade -y && reboot
```

**Installation:**
```bash
wget -q https://github.com/WYCLIFF001/bugsleuth-vpn/releases/download/v0.1.0/installer && chmod +x installer && ./installer
```

---

### Ubuntu 20.04/22.04/24.04 LTS

**First Time Setup:**
```bash
apt-get update && apt-get install -y wget curl && apt-get upgrade -y && apt dist-upgrade -y && update-grub && reboot
```

**Installation:**
```bash
wget -q https://github.com/WYCLIFF001/bugsleuth-vpn/releases/download/v0.1.0/installer && chmod +x installer && ./installer
```

---

### CentOS 8/9 Stream / Rocky Linux 8/9

**First Time Setup:**
```bash
dnf install -y wget curl && dnf update -y && dnf upgrade -y && grub2-mkconfig -o /boot/grub2/grub.cfg && reboot
```

**Installation:**
```bash
wget -q https://github.com/WYCLIFF001/bugsleuth-vpn/releases/download/v0.1.0/installer && chmod +x installer && ./installer
```

---

### Fedora 38/39/40

**First Time Setup:**
```bash
dnf install -y wget curl && dnf update -y && dnf upgrade -y && grub2-mkconfig -o /boot/grub2/grub.cfg && reboot
```

**Installation:**
```bash
wget -q https://github.com/WYCLIFF001/bugsleuth-vpn/releases/download/v0.1.0/installer && chmod +x installer && ./installer
```

---

### AlmaLinux 8/9

**First Time Setup:**
```bash
dnf install -y wget curl && dnf update -y && dnf upgrade -y && grub2-mkconfig -o /boot/grub2/grub.cfg && reboot
```

**Installation:**
```bash
wget -q https://github.com/WYCLIFF001/bugsleuth-vpn/releases/download/v0.1.0/installer && chmod +x installer && ./installer
```

---

### Arch Linux / Manjaro

**First Time Setup:**
```bash
pacman -S --noconfirm wget curl && pacman -Syu --noconfirm && grub-mkconfig -o /boot/grub/grub.cfg && reboot
```

**Installation:**
```bash
wget -q https://github.com/WYCLIFF001/bugsleuth-vpn/releases/download/v0.1.0/installer && chmod +x installer && ./installer
```

---

### openSUSE Leap 15.x / Tumbleweed

**First Time Setup:**
```bash
zypper install -y wget curl && zypper refresh && zypper update -y && zypper dist-upgrade -y && reboot
```

**Installation:**
```bash
wget -q https://github.com/WYCLIFF001/bugsleuth-vpn/releases/download/v0.1.0/installer && chmod +x installer && ./installer
```

---

## [ SERVICES ]

✅ **SSH SERVICES**
- SSH WebSocket TLS & Non-TLS: 443/80
- SSH UDP Custom: 8443
- SSH SSL/TLS: 443

✅ **OPENVPN SERVICES**
- OpenVPN WebSocket TLS & Non-TLS: 443/80
- OpenVPN TCP: 1194
- OpenVPN UDP: 2200
- OpenVPN SSL: 443

✅ **XRAY SERVICES**
- XRAY VMESS WS/gRPC/HTTPUpgrade/XHTTP: 443/80
- XRAY VLESS WS/gRPC/HTTPUpgrade/XHTTP: 443/80
- XRAY TROJAN WS/gRPC/HTTPUpgrade/XHTTP: 443/80

---

## [ OTHER FEATURES ]

✅ Telegram Bot Management<br>
✅ Account Auto-Delete (Expired)<br>
✅ Account Auto-Renewal<br>
✅ BadVPN UDP: 7100-7300<br>
✅ SlowDNS Support<br>
✅ Multi-Protocol Support<br>
✅ Automated Installation<br>
✅ Admin Control Panel<br>

---

```yaml
[ Service & Port Configuration ]

SSH SERVICES:
   - OpenSSH                 : 22
   - SSH WebSocket           : 80, 443
   - SSH WebSocket SSL       : 443
   - SSH UDP Custom          : 8443

OPENVPN SERVICES:
   - OpenVPN WS              : 80
   - OpenVPN WS SSL          : 443
   - OpenVPN TCP             : 1194
   - OpenVPN UDP             : 2200
   - OpenVPN SSL             : 443

XRAY SERVICES:
   - VLESS WS/gRPC           : 443/80
   - VLESS HTTPUpgrade       : 443/80
   - VLESS XHTTP             : 443/80
   - VMESS WS/gRPC           : 443/80
   - VMESS HTTPUpgrade       : 443/80
   - VMESS XHTTP             : 443/80
   - TROJAN WS/gRPC          : 443/80
   - TROJAN HTTPUpgrade      : 443/80
   - TROJAN XHTTP            : 443/80

OTHER SERVICES:
   - BadVPN UDP              : 7100, 7200, 7300
   - SlowDNS                 : Supported

XRAY TRANSPORT MODES:
   - WebSocket (WS)          : ✅
   - gRPC                    : ✅
   - HTTPUpgrade             : ✅
   - XHTTP (Reality)         : ✅
   - XHTTP (Vision)          : ✅
   - XHTTP (SplitHTTP)       : ✅
```

---

## 🤖 Telegram Bot Commands

```
/start  - Start bot & show main menu
/help   - Display help guide
/cancel - Cancel current operation
```

**Main Features:**
- 🔐 SSH Account Management (Create/Delete/Renew/List)
- 🚀 XRAY Account Management (VLESS/VMESS/TROJAN)
- ℹ️ Server Information
- 👥 Admin Management

**Account Creation Format:**
```
SSH    : username:password:days
XRAY   : username:days
Delete : password (SSH) / UUID (XRAY)
Renew  : password:days (SSH) / UUID:days (XRAY)
```

---

## 🔒 Post Installation

**Required Open Ports (Cloud Firewall):**
```
22, 80, 443, 1194, 2200, 8443
```

**Verify Services:**
```bash
systemctl status ssh
systemctl status openvpn
systemctl status xray
```

---

## ⚠️ Important Notes

- Script requires **systemd** support
- Domain must be configured before installation
- Keep Telegram bot token secure
- Regular backups recommended
- Monitor server resources

---

## 📞 Support

Issues? Check [existing issues](../../issues) or [create new one](../../issues/new)

---

<p align="center">
<b>Made with ❤️ for the Community</b><br>
⭐ Star this repo if you find it useful!
</p>
