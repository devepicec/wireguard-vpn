# WireGuard installer

![Lint](https://github.com/angristan/wireguard-install/workflows/Lint/badge.svg)
![visitors](https://visitor-badge.glitch.me/badge?page_id=angristan.wireguard-install)
[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/angristan)

## Requirements

Supported distributions:

- Ubuntu >= 16.04
- Debian >= 10
- Fedora
- CentOS
- AlmaLinux
- Arch Linux
- Oracle Linux

## Usage

Download and execute the script. Answer the questions asked by the script and it will take care of the rest.


## Modo VPN sin enrutamiento
```shell
sudo su
cd
mkdir vpn
curl -O https://raw.githubusercontent.com/devepicec/wireguard-vpn/main/vpn-ep.sh
chmod +x vpn-ep.sh
./vpn-ep.sh
```

## Modo VPN
```shell
sudo su
cd
mkdir vpn
curl -O https://raw.githubusercontent.com/devepicec/wireguard-vpn/main/vpn.sh
chmod +x vpn.sh
./vpn.sh
```


# Para conectarse al VPN

## Modo VPN_EPNet
```bash
sudo su
sudo apt install wireguard
nano /etc/wg10.conf
sudo systemctl enable wg-quick@wg10
sudo systemctl start wg-quick@wg10
sudo systemctl status wg-quick@wg10
```
