### **Hacking Wi-Fi/Kismet.md**

# Kismet

## Descripción

`Kismet` es una herramienta de detección y monitoreo de redes inalámbricas. Funciona como un sniffer pasivo que detecta redes Wi-Fi, dispositivos conectados y recopila información detallada sin interactuar directamente con las redes.

## Uso

```bash
kismet [opciones]
```

### Opciones principales

- `-c`: Define la interfaz de red a utilizar.
- `-t`: Especifica el tipo de captura (e.g., GPS).
- `-u`: Define el usuario propietario de Kismet.
- `-p`: Especifica el puerto para la interfaz web.

## Ejemplos

- Iniciar Kismet en una interfaz específica:

  ```bash
  kismet -c wlan0mon
  ```

- Ejecutar Kismet con interfaz web en el puerto 2501:

  ```bash
  kismet -c wlan0mon -p 2501
  ```

- Iniciar Kismet con soporte GPS:

  ```bash
  kismet -c wlan0mon -t gps
  ```
