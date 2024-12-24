### **Wireless/MDK3/mdk3.md**

# MDK3

## Descripción

`MDK3` es una herramienta de pruebas de estrés para redes Wi-Fi que permite realizar una variedad de ataques, como desautenticación de clientes, inundación de SSID y escaneo de redes. Es útil para evaluar la resistencia de una red inalámbrica frente a diferentes tipos de ataques.

## Uso

```bash
mdk3 interfaz modo [opciones]
```

### Modos principales

- `a`: Ataques de desautenticación.
- `b`: Fuzzing de SSID.
- `c`: Inundación de clientes.
- `d`: Escaneo de redes.
- `s`: Inundación de SSID.

### Opciones principales

- `-c canal`: Especifica el canal en el que se realizará el ataque.
- `-t tiempo`: Define la duración del ataque en segundos.
- `-f archivo_fuzz`: Usa un archivo personalizado para el ataque de fuzzing.
- `--help`: Muestra la ayuda y las opciones disponibles.

## Ejemplos

- Realizar un ataque de desautenticación en el canal 6 durante 60 segundos:

  ```bash
  mdk3 wlan0mon a -c 6 -t 60
  ```

- Inundar SSIDs utilizando un archivo personalizado:

  ```bash
  mdk3 wlan0mon s -f ssids.txt
  ```

- Escanear redes en el canal 11:

  ```bash
  mdk3 wlan0mon d -c 11
  ```
