### **Básico/Miscelánea/od.md**

# od

## Descripción

`od` muestra el contenido de archivos en varios formatos, como octal, hexadecimal y ASCII.

## Uso

od [opciones] archivo

### Opciones principales

- `-t tipo`: Especifica el tipo de salida (e.g., x para hexadecimal).
- `-A formato`: Formato de dirección (n, o, x, d).
- `-j N`: Omite N bytes al inicio.
- `-N N`: Procesa solo N bytes.

## Ejemplos

- Mostrar en hexadecimal:

  od -t x1 archivo.bin

- Mostrar en caracteres ASCII:

  od -c archivo.bin
