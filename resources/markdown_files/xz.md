### **Básico/Compresión y Archivado/xz.md**

# xz

## Descripción

`xz` es una herramienta de compresión que ofrece una alta relación de compresión y es eficiente para comprimir archivos grandes. Utiliza el formato `.xz` y es conocido por su rendimiento en términos de compresión y descompresión.

## Uso

```bash
xz [opciones] archivo
```

### Opciones principales

- `-d` o `--decompress`: Descomprime el archivo.
- `-k` o `--keep`: Mantiene el archivo original después de la compresión/descompresión.
- `-v` o `--verbose`: Modo detallado, muestra el progreso de las operaciones.
- `-r` o `--recursive`: Aplica la operación de forma recursiva a directorios.
- `-c` o `--stdout`: Escribe la salida en la salida estándar.
- `-T`: Define el número de hilos para la compresión.
- `-0` a `-9`: Define el nivel de compresión (0-9).

## Ejemplos

- Comprimir un archivo:
  
  ```bash
  xz archivo.txt
  ```

- Descomprimir un archivo:
  
  ```bash
  xz -d archivo.txt.xz
  ```

- Comprimir manteniendo el archivo original:
  
  ```bash
  xz -k archivo.txt
  ```

- Comprimir con un nivel de compresión alto:
  
  ```bash
  xz -9 archivo.txt
  ```

- Comprimir utilizando múltiples hilos:
  
  ```bash
  xz -T4 archivo.txt
  ```

- Comprimir y escribir la salida en otro archivo:
  
  ```bash
  xz -c archivo.txt > archivo.txt.xz
  ```