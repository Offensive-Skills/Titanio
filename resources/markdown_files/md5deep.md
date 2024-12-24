### **Básico/Encriptación y Hashing/md5deep.md**

# md5deep

## Descripción

`md5deep` calcula sumas de comprobación MD5 de archivos de forma recursiva, útil para analizar grandes conjuntos de datos.

## Uso

md5deep [opciones] [archivos/directorios]

### Opciones principales

- `-r`: Procesa directorios de forma recursiva.
- `-l`: Sigue enlaces simbólicos.
- `-o`: Ordena la salida.
- `-s`: Suprime errores de permiso.
- `-c`: Compara los hashes con una lista conocida.

## Ejemplos

- Calcular hashes MD5 recursivamente en un directorio:

  md5deep -r carpeta/

- Comparar hashes con una lista conocida:

  md5deep -r -c hashes_conocidos.md5 carpeta/

- Generar una lista de hashes MD5:

  md5deep -r carpeta/ > hashes.md5
