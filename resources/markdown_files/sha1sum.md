### **Básico/Encriptación y Hashing/sha1sum.md**

# sha1sum

## Descripción

`sha1sum` calcula y verifica sumas de comprobación SHA-1 para archivos, útil para verificar la integridad de datos.

## Uso

sha1sum [opciones] [archivo]

### Opciones principales

- `-b`: Lee los archivos en modo binario.
- `-c`: Verifica sumas de comprobación desde un archivo.
- `-t`: Lee los archivos en modo texto.
- `--quiet`: Solo muestra mensajes de error.
- `--status`: No muestra ningún mensaje, solo devuelve códigos de salida.

## Ejemplos

- Calcular el hash SHA-1 de un archivo:

  sha1sum archivo.txt

- Verificar sumas de comprobación desde un archivo:

  sha1sum -c checksums.sha1

- Generar sumas SHA-1 para múltiples archivos:

  sha1sum archivo1.txt archivo2.txt > checksums.sha1
