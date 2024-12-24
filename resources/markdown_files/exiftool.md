### **Análisis y Extracción/ExifTool.md**

# ExifTool

## Descripción

`ExifTool` es una poderosa herramienta para leer, escribir y editar metadatos en una amplia variedad de archivos, incluyendo imágenes, audio y video. Es ampliamente utilizada para la manipulación y análisis de metadatos.

## Uso

```bash
exiftool [opciones] [archivo]
```

### Opciones principales

- `-b`: Extrae datos binarios.
- `-s`: Muestra solo los valores sin etiquetas.
- `-all`: Muestra todos los metadatos.
- `-all:all`: Muestra todos los metadatos de todas las categorías.
- `-overwrite_original`: Sobrescribe el archivo original al editar.
- `-r`: Procesa directorios de forma recursiva.
- `-common_args`: Utiliza argumentos comunes de metadatos.

## Ejemplos

- Mostrar todos los metadatos de una imagen:

  ```bash
  exiftool imagen.jpg
  ```

- Extraer la fecha de creación de un archivo:

  ```bash
  exiftool -CreateDate archivo.png
  ```

- Eliminar todos los metadatos de una imagen:

  ```bash
  exiftool -all= imagen.jpg
  ```

- Copiar metadatos de una imagen a otra:

  ```bash
  exiftool -TagsFromFile fuente.jpg -all:all destino.jpg
  ```

- Guardar todos los metadatos en un archivo de texto:

  ```bash
  exiftool imagen.jpg > metadatos.txt
  ```
