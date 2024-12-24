### **Análisis de Tráfico Web/Wireshark.md**

# Wireshark

## Descripción

`Wireshark` es un analizador de protocolos de red de código abierto. Permite capturar y explorar el tráfico de red en tiempo real, proporcionando una profunda comprensión de lo que ocurre en la red a nivel de protocolos.

## Uso

```bash
wireshark [opciones]
```

### Opciones principales

- `-i`: Especifica la interfaz de red para capturar paquetes.
- `-k`: Inicia la captura inmediatamente.
- `-f`: Define un filtro de captura (usando la sintaxis de pcap).
- `-Y`: Aplica un filtro de visualización.
- `-w`: Guarda la captura en un archivo.
- `-r`: Lee paquetes desde un archivo guardado.
- `-h`: Muestra ayuda y opciones disponibles.

## Ejemplos

- Iniciar Wireshark y capturar en la interfaz eth0:

  ```bash
  wireshark -i eth0
  ```

- Capturar paquetes HTTP y guardar en un archivo:

  ```bash
  wireshark -i eth0 -k -f "tcp port 80" -w captura_http.pcap
  ```

- Leer y analizar una captura guardada:

  ```bash
  wireshark -r captura_http.pcap
  ```

- Aplicar un filtro de visualización para mostrar solo tráfico HTTPS:

  ```bash
  wireshark -Y "ssl"
  ```
