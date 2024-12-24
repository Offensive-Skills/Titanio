### **Básico/Compresión y Archivado/bzip2.md**

# bzip2

## Descripción

`bzip2` es una herramienta de compresión que ofrece una mejor relación de compresión que `gzip` a costa de un mayor uso de recursos. Es comúnmente utilizada para comprimir archivos individuales, resultando en archivos con la extensión `.bz2`.

## Uso

```bash
bzip2 [opciones] archivo
```

### Opciones principales

- `-d`: Descomprime el archivo.
- `-k`: Mantiene el archivo original después de la compresión/descompresión.
- `-v`: Modo detallado, muestra el progreso de las operaciones.
- `-r`: Aplica la operación de forma recursiva a directorios.
- `-c`: Escribe la salida en la salida estándar.
- `-1` a `-9`: Define el nivel de compresión (1-9).

## Ejemplos

- Comprimir un archivo:
  
  ```bash
  bzip2 archivo.txt
  ```

- Descomprimir un archivo:
  
  ```bash
  bzip2 -d archivo.txt.bz2
  ```

- Comprimir manteniendo el archivo original:
  
  ```bash
  bzip2 -k archivo.txt
  ```

- Comprimir con un nivel de compresión alto:
  
  ```bash
  bzip2 -9 archivo.txt
  ```

- Comprimir todos los archivos en un directorio de forma recursiva:
  
  ```bash
  bzip2 -r carpeta/
  ```

- Comprimir y escribir la salida en otro archivo:
  
  ```bash
  bzip2 -c archivo.txt > archivo.txt.bz2
  ```