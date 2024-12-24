### **Hacking Wi-Fi/Aircrack-ng.md**

# Aircrack-ng

## Descripción

`Aircrack-ng` es un conjunto de herramientas para evaluar la seguridad de redes Wi-Fi. Permite la captura de paquetes, la inyección de tráfico y el análisis de contraseñas mediante ataques de fuerza bruta sobre archivos de captura.

## Uso

```bash
aircrack-ng [opciones] archivo.cap
```

### Opciones principales

- `-a`: Define el modo de ataque (e.g., WPA, WEP).
- `-b`: Especifica el BSSID del objetivo.
- `-w`: Define el archivo de diccionario para ataques de fuerza bruta.
- `-c`: Especifica el canal de la red.
- `-e`: Define el ESSID de la red.

## Ejemplos

- Descifrar una clave WEP:

  ```bash
  aircrack-ng -a 1 -b 00:11:22:33:44:55 -w diccionario.txt captura.cap
  ```

- Realizar un ataque de fuerza bruta en WPA:

  ```bash
  aircrack-ng -a 2 -b 00:11:22:33:44:55 -w rockyou.txt captura.cap
  ```

- Escanear redes Wi-Fi cercanas:

  ```bash
  airodump-ng wlan0mon
  ```

