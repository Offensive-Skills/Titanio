### **Análisis de Red/NetworkMiner/networkminer.md**

# NetworkMiner

## Descripción

**NetworkMiner** es una herramienta de análisis forense de red (NFAT) que puede detectar sistemas operativos, sesiones, nombres de host y extraer archivos sin poner el tráfico en riesgo. Es útil para analizar archivos PCAP y realizar análisis pasivos de red.

## Uso

NetworkMiner es una aplicación gráfica disponible para Windows y Linux (usando Mono).

### Características principales

- **Análisis pasivo**: No envía paquetes, solo analiza lo capturado.
- **Extracción de archivos**: Recupera archivos transferidos por HTTP, FTP, etc.
- **Detección de sistemas operativos**: Identifica SO basándose en patrones de tráfico.
- **Visualización de sesiones**: Muestra conexiones y flujos de datos.

## Ejemplos de uso

- **Abrir un archivo PCAP**:

  - Iniciar NetworkMiner.
  - Seleccionar "File" > "Open" y elegir el archivo PCAP.

- **Analizar tráfico en vivo**:

  - Seleccionar la interfaz de red.
  - Hacer clic en "Start" para comenzar la captura.

