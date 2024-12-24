### **Análisis Forense/Binwalk/binwalk.md**

# Binwalk

## Descripción

`binwalk` es una herramienta para analizar y extraer datos de archivos binarios. Está diseñada para la ingeniería inversa de firmware, permitiendo identificar firmas, archivos embebidos y código ejecutable dentro de imágenes binarias.

## Uso

```bash
binwalk [opciones] archivo
```

### Opciones principales

- `-e`: Extrae automáticamente los datos identificados.
- `-D 'tipo':directorio`: Extrae datos de un tipo específico a un directorio.
- `-M`: Modo recursivo, analiza los archivos extraídos.
- `-B`: Busca opcodes de código ejecutable.
- `-r`: Utiliza expresiones regulares personalizadas.

## Ejemplos

- Analizar un archivo binario:

  ```bash
  binwalk firmware.bin
  ```

- Extraer contenido embebido:

  ```bash
  binwalk -e firmware.bin
  ```

- Análisis recursivo:

  ```bash
  binwalk -Me firmware.bin
  ```

