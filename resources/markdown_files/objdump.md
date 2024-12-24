### **Binary_Analysis/Objdump/objdump.md**

# Objdump

## Descripción

`objdump` es una herramienta de línea de comandos que permite desensamblar y analizar archivos binarios. Forma parte del conjunto de herramientas GNU Binutils y es ampliamente utilizada para examinar el contenido de ejecutables, bibliotecas y otros formatos de archivo binario.

## Uso

```bash
objdump [opciones] archivo_binario
```

### Opciones principales

- `-d`: Desensambla todas las secciones de código ejecutable.
- `-D`: Desensambla todas las secciones, incluyendo no ejecutables.
- `-x`: Muestra toda la información de encabezado y secciones.
- `-t`: Lista la tabla de símbolos del archivo.
- `-s`: Muestra el contenido hexadecimal de las secciones.
- `-C`: Desenmama símbolos con nombres más legibles (demangle).

## Ejemplos

- Desensamblar las secciones de código ejecutable de un binario:

  ```bash
  objdump -d archivo.bin
  ```

- Desensamblar todas las secciones, incluyendo datos:

  ```bash
  objdump -D archivo.bin
  ```

- Mostrar la tabla de símbolos de un binario:

  ```bash
  objdump -t archivo.bin
  ```

- Mostrar toda la información de encabezado y secciones:

  ```bash
  objdump -x archivo.bin
  ```

- Desensamblar y demangle los símbolos:

  ```bash
  objdump -dC archivo.bin
  ```
