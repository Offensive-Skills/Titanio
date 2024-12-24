### **Mobile_Security/Needle/needle.md**

# Needle

## Descripción

`Needle` es una plataforma de pruebas de penetración para aplicaciones iOS que automatiza el proceso de análisis de seguridad, facilitando la identificación y explotación de vulnerabilidades en aplicaciones móviles.

## Uso

```bash
needle scan --app app.ipa --device <device_id>
```

### Opciones principales

- `scan`: Inicia un escaneo de seguridad en la aplicación.
- `--app`: Especifica el archivo IPA de la aplicación a analizar.
- `--device`: Define el ID del dispositivo iOS conectado.
- `--report`: Guarda el informe de análisis en un archivo.
- `--verbose`: Muestra información detallada durante el escaneo.

## Ejemplos

- **Escanear una aplicación iOS y generar un informe:**
  
  ```bash
  needle scan --app app.ipa --device ABC123 --report informe_needle.html
  ```

- **Ejecutar un escaneo detallado:**
  
  ```bash
  needle scan --app app.ipa --device ABC123 --verbose
  ```

- **Listar dispositivos iOS conectados:**
  
  ```bash
  needle list_devices
  ```
