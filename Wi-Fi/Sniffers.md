# Sniffers

## Probe Request Sniff

El Probe Request Sniff nos muestra los distintos dispositivos que se intentan conectar a las distintas redes Wi-Fi que se encuentran a nuestro alrededor. Los números que se encuentran a la izquierda son las direcciones MAC de los dispositivos que se intentan conectar a las redes Wi-Fi y a la derecha el BSSID de la red Wi-Fi a la que se intentan conectar.

## Beacon Sniff

Nos permite detectar todos los beacons que hay en la red y el BSSID que está emitiendo el beacon. Esto es bastante útil para analizar las redes que están teniendo tráfico en este momento.

## Deauth Sniff

Nos permite detectar distintos ataques Deauth en nuestro entorno. Podemos ver todos los paquetes que se están enviando en el ataque.

## Packet Count

Esta técnica nos permite ver la cantidad de tramas Wi-Fi recibidas de un punto de acceso o dispositivo seleccionado.

## EAPOL/PMKID Scan

Esta técnica es muy útil ya que nos permite capturar tramas de autenticación Wi-Fi en tiempo real.

- **EAPOL**: es el protocolo que usan los dispositivos para iniciar la conexión segura con un router Wi-Fi.
- **PMKID**: es un código especial que viaja en los primeros mensajes de conexión y que nos sirve para descubrir la contraseña de la red.

## Packet Monitor

Esta técnica nos permite monitorear todos los paquetes en bruto. Se divide en tres colores: el verde, donde podemos ver los beacon; el rojo, los ataques Deauth; y en azul, los probes.

## Channel Analyzer

Nos detecta el tráfico que está habiendo entre los distintos canales de red. Esta opción nos muestra los datos en bruto y nos daría información de en qué canales se está moviendo el tráfico de red.

## Channel Summary

Nos muestra un gráfico con el número de dispositivos conectados a un canal en concreto. Esta técnica nos sirve para detectar el tipo de canales que utilizan todos los dispositivos conectados a una red.

## Raw Capture

Esta técnica captura y muestra paquetes de Wi-Fi en bruto (en formato .pcap) directamente en la tarjeta Micro SD para su posterior análisis.

## Detect Pwnagotchi

Esta técnica nos permite buscar y escanear dispositivos Pwnagotchi cercanos en el aire.

## Detect Pineapple

Esta técnica nos permite detectar dispositivos Wi-Fi Pineapple (estos son dispositivos de hardware especializado para auditar redes inalámbricas y realizar pruebas de hacking ético).

## Detect MultiSSID

Esta técnica nos va a permitir saber si un mismo punto de acceso está transmitiendo múltiples redes Wi-Fi (SSID) a la vez.

## Scan AP/STA

Esta técnica nos permite ver las redes Wi-Fi que se encuentran a nuestro alcance. Podemos diferenciar dos colores: el verde, que nos indica las redes Wi-Fi que tenemos disponibles, y en azul los distintos dispositivos que se encuentran en las diferentes redes Wi-Fi.

## Fox Hunt

Es una técnica que nos permite rastrear la fuente o intensidad de una señal inalámbrica específica moviéndose según la potencia de recepción, imitando el juego tradicional de orientación por radiogoniometría de "la caza del zorro".

## MAC Monitor

Esta técnica nos permite rastrear y monitorizar direcciones MAC en tiempo real a nuestro alrededor.

## SAE Commit

Es una técnica que tiene como función la captura de tráfico Wi-Fi y filtra tramas de autenticación del protocolo WPA3 (SAE).

- **Protocolo SAE (Simultaneous Authentication of Equals)**: es el método que usa WPA3 para conectar dispositivos de forma segura y evitar que intercepten la contraseña.

## Wardrive

Esta técnica se trata de la detección de dispositivos Bluetooth al igual que de redes Wi-Fi mientras nos encontramos circulando en coche por un área que queramos analizar.

### Análisis del Wardrive

Para comenzar con este ejercicio debemos insertar la tarjeta SD en nuestro ordenador. Una vez dentro podremos ver diferentes tipos de archivos: ap_sta (puntos de acceso), beacon, Deauth y el más importante, que es el archivo de wardrive al final de todo. Este documento se encuentra escrito en texto claro y en formato WiggleWifi. Dentro de este archivo podemos encontrar a la izquierda todos los BSSID recolectados y las direcciones de los dispositivos Bluetooth junto a unas coordenadas GPS.

Para poder verlo de manera gráfica podemos emplear la herramienta Wardrive-Tracker de afsh4ck. Esta herramienta funciona tanto para Windows como para Linux, siempre y cuando tengamos instalado Python. Una opción destacable es la que se encuentra arriba a la derecha (geolocalizar/refinar BSSID), la cual nos dará el punto exacto del dispositivo.
