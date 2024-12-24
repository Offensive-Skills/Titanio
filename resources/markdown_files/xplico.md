### **Análisis de Red/Xplico/xplico.md**

# Xplico

## Descripción

**Xplico** es una herramienta de análisis forense de red que reconstruye los contenidos de las comunicaciones a partir de capturas de tráfico. Puede extraer correos electrónicos, imágenes, llamadas VoIP y más.

## Uso

Xplico se ejecuta como un servicio web al que se accede mediante un navegador.

### Características principales

- **Reensamblado de datos**: Reconstruye aplicaciones y datos a partir de paquetes.
- **Soporte para múltiples protocolos**: HTTP, SMTP, SIP, TCP, UDP, etc.
- **Interfaz web**: Fácil de usar y gestionar casos.

## Ejemplos de uso

- **Iniciar Xplico**:

  ```bash
  sudo service xplico start
  ```

- **Acceder a la interfaz web**:

  - Abrir `http://localhost:9876` en un navegador.
  - Iniciar sesión con las credenciales por defecto.

- **Crear un nuevo caso y cargar una captura**:

  - Crear un caso desde la interfaz.
  - Subir un archivo PCAP para analizar.
