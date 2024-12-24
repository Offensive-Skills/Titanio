### **Mobile_Security/AndroBios/androbios.md**

# AndroBios

## Descripción

`AndroBios` es una herramienta de análisis de seguridad para dispositivos Android que permite la inspección de la BIOS y otros componentes del sistema para detectar vulnerabilidades y configuraciones inseguras.

## Uso

```bash
androbios [opciones]
```

### Opciones principales

- `-d, --device`: Especifica el dispositivo Android a analizar.
- `-o, --output archivo`: Guarda el informe de análisis en un archivo.
- `-v, --verbose`: Muestra información detallada durante el análisis.
- `-h, --help`: Muestra la ayuda y las opciones disponibles.

## Ejemplos

- **Analizar un dispositivo Android y guardar el informe:**
  
  ```bash
  androbios -d /dev/bus/usb/001/002 -o informe.txt
  ```

- **Ejecutar un análisis detallado:**
  
  ```bash
  androbios -d /dev/bus/usb/001/002 -v
  ```

- **Mostrar ayuda:**
  
  ```bash
  androbios -h
  ```

