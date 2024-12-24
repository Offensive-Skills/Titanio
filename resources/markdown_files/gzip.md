### **Básico/Compresión y Archivado/gzip.md**

# gzip

## Descripción

`gzip` es una herramienta de compresión utilizada para comprimir archivos individuales, reduciendo su tamaño para facilitar el almacenamiento y la transferencia. Generalmente se usa junto con `tar` para comprimir archivos tar en formato `.tar.gz` o `.tgz`.

## Uso

```bash
gzip [opciones] archivo
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
  gzip archivo.txt
  ```

- Descomprimir un archivo:
  
  ```bash
  gzip -d archivo.txt.gz
  ```

- Comprimir manteniendo el archivo original:
  
  ```bash
  gzip -k archivo.txt
  ```

- Comprimir con un nivel de compresión alto:
  
  ```bash
  gzip -9 archivo.txt
  ```

- Comprimir todos los archivos en un directorio de forma recursiva:
  
  ```bash
  gzip -r carpeta/
  ```

- Comprimir y escribir la salida en otro archivo:
  
  ```bash
  gzip -c archivo.txt > archivo.txt.gz
  ```