### **Análisis de Red/tcpdump/tcpdump.md**

# tcpdump

## Descripción

`tcpdump` es una herramienta de línea de comandos que permite capturar y analizar paquetes de red. Es útil para diagnosticar problemas de red, analizar tráfico y depurar aplicaciones que utilizan la red.

## Uso

```bash
tcpdump [opciones] [expresión]
```

### Opciones principales

- `-i interfaz`: Especifica la interfaz de red a utilizar.
- `-w archivo`: Guarda la captura en un archivo.
- `-r archivo`: Lee paquetes de un archivo guardado.
- `-n`: No resuelve nombres de host ni puertos.
- `-v`, `-vv`, `-vvv`: Modo detallado, muestra más información.
- `-c N`: Captura N paquetes y luego sale.

## Ejemplos

- Capturar paquetes en la interfaz eth0:

  ```bash
  tcpdump -i eth0
  ```

- Guardar la captura en un archivo:

  ```bash
  tcpdump -i eth0 -w captura.pcap
  ```

- Capturar paquetes HTTP:

  ```bash
  tcpdump -i eth0 tcp port 80
  ```
