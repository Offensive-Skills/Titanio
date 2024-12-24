### **Básico/Encriptación y Hashing/md5sum.md**

# md5sum

## Descripción

`md5sum` calcula y verifica sumas de comprobación MD5 para archivos, útil para verificar la integridad de datos.

## Uso

md5sum [opciones] [archivo]

### Opciones principales

- `-b`: Lee los archivos en modo binario.
- `-c`: Verifica sumas de comprobación desde un archivo.
- `-t`: Lee los archivos en modo texto.
- `--quiet`: Solo muestra mensajes de error.
- `--status`: No muestra ningún mensaje, solo devuelve códigos de salida.

## Ejemplos

- Calcular el hash MD5 de un archivo:

  md5sum archivo.txt

- Verificar sumas de comprobación desde un archivo:

  md5sum -c checksums.md5

- Generar sumas MD5 para múltiples archivos:

  md5sum archivo1.txt archivo2.txt > checksums.md5
