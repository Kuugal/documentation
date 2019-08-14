---
title: "OpenVPN GUI"
tags: ["OpenVPN", "VPN"]
menuTitle : "OpenVPN"
---
<img src="/img/openvpn-logo.png" width="720">
### ¿Qué es OpenVPN?
___
Es una herramienta de conectividad basada en software libre: SSL (Secure Sockets Layer), VPN Virtual Private Network (red virtual privada). OpenVPN ofrece conectividad punto-a-punto con validación jerárquica de usuarios y host conectados remotamente.

### Windows
___
1. Descarga e instala la última versión del [WINDOWS INSTALLER (NSIS)](https://openvpn.net/index.php/open-source/downloads.html)

2. Descomprime el archivo **[openvpn-config.zip](/zip/openvpn-config.zip)** y copia los 5 archivos en la ruta donde se ha instalado el programa, *C:\Program Files\OpenVPN\config*

### Linux
___
#### Debian-like

1. Instalación del cliente
```
apt-get install openvpn
```
2. Copia los certificados
```
cp ca.crt nielsen.crt nielsen.key vpn.cnf /etc/openvpn/client
```
3. Accede a */etc/openvpn/client* y cambiamos la extensión del archivo
vpn**.cnf** por **.conf**
4. Iniciar la conexión con el servidor, sobre la ruta ``/etc/openvpn`` ejecuta
```
openvpn /etc/openvpn/client/vpn.conf
```