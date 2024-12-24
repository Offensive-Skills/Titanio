### **Binary_Analysis/Strings/strings.md**

# Strings

## Descripción

`strings` es una herramienta de línea de comandos utilizada para extraer secuencias de texto legible de archivos binarios. Es útil en análisis forense, ingeniería inversa y depuración para identificar cadenas de texto incrustadas, como mensajes de error, nombres de funciones y datos de configuración.

## Uso

```bash
strings [opciones] archivo_binario
```

### Opciones principales

- `-a`: Busca en todo el archivo, no solo en las secciones de datos.
- `-n número`: Define la longitud mínima de las cadenas a extraer (por defecto, 4).
- `-e formato`: Especifica el formato de codificación (s para ASCII, b para binario, etc.).
- `-t x`: Muestra la dirección hexadecimal de cada cadena.
- `-f`: Imprime el nombre del archivo antes de las cadenas.

## Ejemplos

- Extraer todas las cadenas de al menos 6 caracteres:

  ```bash
  strings -n 6 archivo.bin
  ```

- Buscar cadenas en formato hexadecimal con sus direcciones:

  ```bash
  strings -n 5 -t x archivo.bin
  ```

- Extraer cadenas de un archivo específico y guardar en otro archivo:

  ```bash
  strings archivo.bin > cadenas.txt
  ```

- Buscar cadenas en todo el archivo, incluyendo secciones no estándar:

  ```bash
  strings -a archivo.bin
  ```
