### **Reverse_Engineering/Jadx/jadx.md**

# Jadx

## Descripción

`Jadx` es una herramienta de código abierto que permite descompilar archivos APK de Android y archivos DEX a código fuente Java legible. Es útil para desarrolladores y profesionales de seguridad que buscan analizar aplicaciones móviles, identificar vulnerabilidades y entender el funcionamiento interno de las aplicaciones.

## Uso

```bash
jadx [opciones] archivo_apk
```

### Opciones principales

- `-d directorio_salida`: Define el directorio donde se guardará el código fuente descompilado.
- `-r`: Incluye recursos y archivos adicionales en la salida.
- `-j núcleos`: Especifica el número de núcleos de CPU a utilizar para la descompilación.
- `--show-bad-code`: Muestra el código que no pudo ser descompilado correctamente.
- `-h`: Muestra la ayuda y las opciones disponibles.

## Ejemplos

- Descompilar un archivo APK y guardar el código fuente en un directorio específico:

  ```bash
  jadx -d salida_codigo ./app.apk
  ```

- Descompilar un archivo APK con múltiples núcleos de CPU para mayor velocidad:

  ```bash
  jadx -d salida_codigo -j 4 ./app.apk
  ```

- Incluir recursos adicionales en la salida descompilada:

  ```bash
  jadx -d salida_codigo -r ./app.apk
  ```

- Mostrar código que no pudo ser descompilado correctamente:

  ```bash
  jadx --show-bad-code ./app.apk
  ```
