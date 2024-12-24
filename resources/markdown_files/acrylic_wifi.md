### **Wireless/Acrylic_Wifi/acrylic_wifi.md**

# Acrylic Wi-Fi

## Descripción

`Acrylic Wi-Fi` es una herramienta de análisis y auditoría de redes inalámbricas que permite escanear, monitorizar y evaluar la seguridad de redes Wi-Fi. Ofrece visualización de canales, identificación de puntos de acceso y detección de dispositivos conectados.

## Uso

```bash
acrylic_wifi [opciones]
```

### Opciones principales

- `-s`: Inicia un escaneo de redes Wi-Fi.
- `-c canal`: Especifica el canal para el escaneo.
- `-o archivo_salida`: Guarda los resultados del escaneo en un archivo.
- `-v`: Modo detallado, muestra información adicional.
- `--help`: Muestra la ayuda y las opciones disponibles.

## Ejemplos

- Escanear redes Wi-Fi en el canal 11:

  ```bash
  acrylic_wifi -s -c 11
  ```

- Guardar los resultados del escaneo en un archivo:

  ```bash
  acrylic_wifi -s -o resultados.txt
  ```

- Iniciar un escaneo detallado:

  ```bash
  acrylic_wifi -s -v
  ```

