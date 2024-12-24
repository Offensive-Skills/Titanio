### **Análisis de Tráfico Web/mitmproxy.md**

# mitmproxy

## Descripción

`mitmproxy` es una herramienta de proxy de intercepción que permite inspeccionar, modificar y reproducir el tráfico HTTP y HTTPS. Es útil para desarrolladores y testers de seguridad que necesitan analizar y manipular el tráfico entre clientes y servidores.

## Uso

```bash
mitmproxy [opciones]
```

### Opciones principales

- `-p`: Define el puerto en el que mitmproxy escuchará (por defecto 8080).
- `-r`: Lee y reproduce una captura de tráfico desde un archivo.
- `-w`: Guarda el tráfico capturado en un archivo.
- `-s`: Ejecuta un script específico para modificar el tráfico.
- `--mode`: Define el modo de operación (e.g., regular, transparent, reverse).

## Ejemplos

- Iniciar mitmproxy en el puerto 8080:

  ```bash
  mitmproxy -p 8080
  ```

- Guardar el tráfico capturado en un archivo:

  ```bash
  mitmproxy -w captura_trafico.mitm
  ```

- Leer y reproducir tráfico desde un archivo:

  ```bash
  mitmproxy -r captura_trafico.mitm
  ```

- Ejecutar un script para modificar solicitudes:

  ```bash
  mitmproxy -s modificar_solicitudes.py
  ```
