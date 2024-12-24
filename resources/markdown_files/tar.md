### **Básico/Compresión y Archivado/tar.md**

# tar

## Descripción

`tar` es una herramienta utilizada para agrupar múltiples archivos y directorios en un solo archivo, conocido como archivo tar o tarball. También puede comprimir y descomprimir archivos tar utilizando diferentes algoritmos de compresión.

## Uso

```bash
tar [opciones] archivo.tar [archivos/directorios]
```

### Opciones principales

- `-c`: Crea un nuevo archivo tar.
- `-x`: Extrae archivos de un archivo tar.
- `-t`: Lista el contenido de un archivo tar.
- `-v`: Modo detallado, muestra el progreso de las operaciones.
- `-f`: Especifica el nombre del archivo tar.
- `-z`: Comprime o descomprime usando gzip.
- `-j`: Comprime o descomprime usando bzip2.
- `-J`: Comprime o descomprime usando xz.
- `-C`: Cambia al directorio especificado antes de realizar operaciones.

## Ejemplos

- Crear un archivo tar:
  
  ```bash
  tar -cf archivo.tar carpeta/
  ```

- Crear un archivo tar comprimido con gzip:
  
  ```bash
  tar -czf archivo.tar.gz carpeta/
  ```

- Listar el contenido de un archivo tar:
  
  ```bash
  tar -tf archivo.tar
  ```

- Extraer un archivo tar:
  
  ```bash
  tar -xf archivo.tar
  ```

- Extraer un archivo tar comprimido con bzip2 en un directorio específico:
  
  ```bash
  tar -xjf archivo.tar.bz2 -C /ruta/destino/
  ```