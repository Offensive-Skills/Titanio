### **Básico/Miscelánea/du.md**

# du

## Descripción

`du` estima el uso del espacio en disco de archivos y directorios.

## Uso

du [opciones] [archivo/directorio]

### Opciones principales

- `-h`: Muestra tamaños en formato legible.
- `-s`: Muestra un resumen del tamaño total.
- `-a`: Incluye archivos en el reporte.
- `-d N`: Profundidad máxima de directorios.

## Ejemplos

- Mostrar el tamaño de un directorio:

  du -h carpeta/

- Mostrar el tamaño total de un directorio:

  du -sh carpeta/

- Mostrar tamaños hasta una profundidad de 1 nivel:

  du -h -d 1 carpeta/
