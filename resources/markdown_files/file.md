### **Básico/Miscelánea/file.md**

# file

## Descripción

`file` determina el tipo de un archivo examinando su contenido.

## Uso

file [opciones] archivo

### Opciones principales

- `-b`: Muestra solo el tipo de archivo, sin el nombre.
- `-i`: Muestra el tipo MIME del archivo.
- `-z`: Examina el contenido dentro de archivos comprimidos.

## Ejemplos

- Determinar el tipo de un archivo:

  file archivo.txt

- Mostrar solo el tipo MIME:

  file -i imagen.jpg
