# Scanners

Para poder usar esta opción es importante que el dispositivo se encuentre conectado con la red wifi objetivo.

## Ping Scan

Esta opción nos permite comprobar qué dispositivos están accesibles o en una red. El proceso es sencillo, el dispositivo envía solicitudes ICMP Echo Request (ping) a distintas direcciones Ip, si un dispositivo responde quiere decir que esta accesible.

## ARP Scan

Esta técnica nos permite buscar dispositivos dentro de la misma red local empleando el protocolo ARP (Adress Resolution Protocol). Si algún dispositivo responde, podemos obtener información como dirección IP y la dirección MAC

## Port Scan all

Esta opción permite comprobar que puertos de red están abiertos en un dispositivo, gracias a esto podremos ver que servicio esta escuchando.

⚠️ Este tipo de escaneo puede generar bastante tráfico y por ende ser detectado por sistemas de seguridad

## SSH Scan

Esta técnica nos permite detectar dispositivos que posean el servicio SSH (Secure Shell) disponible. Esta técnica no implica iniciar sesión ni obtener acceso.

## Telnet Scan

El Telnet Scan nos permite detectar dispositivos con el servicio Telnet corriendo, este servicio, nos permite el acceso remoto mediante texto pero no cifra la comunicación, por lo que actualmente se considera inseguro para muchos usos

## SMTP Scan

Busca dispositivos que posean el SMTP (Simple Mail Transfer Protocol) abierto. Este servicio como bien sabemos nos permite principalmente para el envío de correo electrónico.

## DNS Scan

Busca dispositivos que ofrezcan un servicio DNS (Domain Name System), estos dispositivos suelen ser Routers, Servidores DNS internos y públicos.

## HTTP Scan

Busca servidores web que respondan mediante HTTP

## HTTPS Scan

Busca servidores web que respondan mediante HTTPS

## RDP Scan

Busca dispositivos que tengan disponible RDP (Remote Desktop Protocol). Normalmente este servicio se emplea para controlar equipos Windows de forma remota mediante una interfaz gráfica.
