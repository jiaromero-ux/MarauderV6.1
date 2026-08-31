# ESP32 Marauder V6.1 - Guía de Funciones (Español)

## 🎯 Motivación

Al empezar a trastear con el ESP32 Marauder V6.1 no encontré apenas ninguna guía en español que explicara de forma clara y resumida para qué sirve cada función del dispositivo. Es por ello, por lo que decidí crear esta guía, para que a la gente que está comenzando a emplear este dispositivo no le pase lo mismo.

> ⚠️ **Uso educativo y de auditoría autorizada.** El uso sin consentimiento sobre redes o dispositivos de terceros puede ser ilegal.

---

## 📂 Contenido

- **📶 WiFi**
  - [Sniffers](./wifi/sniffers.md)
  - [Scanners](./wifi/scanners.md)
  - [Attacks](./wifi/attacks.md)

- **📡 Bluetooth**
  - [Sniffers](./bluetooth/sniffers.md)
  - [Attacks](./bluetooth/attacks.md)

- **🛰️ GPS**
  - [GPS Data](./gps/gps-data.md)
  - [NMEA Stream](./gps/nmea-stream.md)
  - [GPS Tracker](./gps/gps-tracker.md)
  - [GPS POI](./gps/gps-poi.md)

- **⚙️ Device**
  - [Device](./device/device.md)

---

## 📶 WiFi

Para realizar auditorías WiFi, el dispositivo posee un apartado de WiFi, el cual posee 4 opciones, las cuales iremos desglosando a medida que vayamos avanzando. Las opciones que podemos observar son:

- **Sniffers**: también conocidos como analizador de paquetes o monitor de red, son herramientas que nos permiten capturar y analizar el tráfico que circula por una red.
- **Scanners**: son herramientas que nos permitirán escanear diferentes protocolos dentro de una red WiFi.
- **Attacks**: nos permitirá realizar diferentes ataques WiFi.

---

## 📡 Bluetooth

Para realizar auditorías Bluetooth, el dispositivo posee un apartado 'Bluetooth', el cual posee 2 opciones, las cuales iremos desglosando a medida que vayamos avanzando. Las opciones que podemos observar son:

- **Sniffers**: también conocidos como analizador de paquetes o monitor de red, son herramientas que nos permiten capturar y analizar tráfico Bluetooth.
- **Attacks**: nos permitirá realizar diferentes ataques Bluetooth.

### Bluetooth Analyzer

Técnica que permite escanear, capturar y analizar el entorno de radiofrecuencia Bluetooth, así como realizar pruebas de seguridad sobre los dispositivos detectados.

### Flock Sniff

Función de escaneo inalámbrico utilizada para detectar cámaras de vigilancia de la marca Flock Safety.

### Meta Detect

Función que permite escanear y localizar dispositivos de la marca Meta (incluidos los que incorporan IA, como las gafas inteligentes).

### Fox Hunt

Función de localización por intensidad de señal (RSSI) que permite rastrear físicamente un dispositivo Bluetooth hasta encontrarlo, mostrando en tiempo real si te acercas o alejas según la potencia de la señal recibida.

### FindMy Sound Attack

Función que explota el protocolo Find My de Apple: el dispositivo emite anuncios BLE falsificados imitando un AirTag, lo que puede provocar que dispositivos Apple cercanos detecten un "accesorio desconocido" o que un accesorio real emita sonido de localización.

---

## 🛰️ GPS

Para realizar auditorías GPS, el dispositivo posee un apartado 'GPS', el cual posee 4 opciones. Las opciones que podemos observar son:

### GPS Data

Función que integra un módulo GPS externo (vía UART) para añadir geolocalización a los escaneos y capturas realizados con Marauder.

### NMEA Stream

Muestra en tiempo real las tramas NMEA que envía el módulo GPS (latitud, longitud, altitud, hora UTC, satélites), sin procesarlas ni asociarlas a otros escaneos.

### GPS Tracker

Registra la posición actual de forma continua y la guarda en la SD, generando un histórico del recorrido físico realizado (track/ruta).

### GPS POI

Permite marcar y guardar puntos de interés (POI) concretos, asociando una ubicación a una etiqueta o nota (por ejemplo, dónde se detectó una red o dispositivo relevante).

---

## ⚙️ Device

Menú de configuración y estado del propio dispositivo, separado de las funciones de escaneo/ataque. Normalmente incluye:

- **Información del sistema**: versión de firmware, chip (ESP32/ESP32-S3), memoria libre, estado de la SD card.
- **Configuración de pantalla**: brillo, orientación, tipo de display conectado.
- **Configuración de red/AP**: nombre del punto de acceso de configuración, credenciales del WebUI.
- **Gestión de batería**: nivel de carga, modo de ahorro de energía (si el hardware lo soporta).
- **Actualización de firmware (OTA)**: flashear nueva versión sin necesidad de cable, si el firmware lo permite.
- **Reset/Reboot**: reiniciar el dispositivo o restaurar configuración de fábrica.

---

📌 *Guía en construcción — se irá ampliando conforme pruebe más funciones del firmware.*
