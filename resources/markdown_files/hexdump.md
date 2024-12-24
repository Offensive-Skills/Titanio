### **Básico/Miscelánea/hexdump.md**

# hexdump

## Descripción

`hexdump` muestra el contenido de archivos en formato hexadecimal.

## Uso

hexdump [opciones] archivo

### Opciones principales

- `-C`: Muestra salida canónica (hexadecimal y ASCII).
- `-n N`: Muestra solo N bytes.
- `-v`: No agrupa líneas idénticas con asteriscos.

## Ejemplos

- Mostrar el contenido en hexadecimal y ASCII:

  hexdump -C archivo.bin

- Mostrar los primeros 64 bytes:

  hexdump -n 64 archivo.bin
