### **Básico/Procesamiento de Texto/cat.md**

# cat

## Descripción

`cat` concatena y muestra el contenido de archivos.

## Uso

```bash
cat [opciones] archivo...
```

### Opciones principales

- `-n`: Numera todas las líneas de la salida.
- `-b`: Numera solo las líneas no vacías.
- `-E`: Muestra un `$` al final de cada línea.
- `-s`: Suprime líneas en blanco repetidas.
- `-T`: Muestra tabulaciones como `^I`.

## Ejemplos

- Mostrar el contenido de un archivo:

  ```bash
  cat archivo.txt
  ```

- Concatenar múltiples archivos y mostrar el resultado:

  ```bash
  cat archivo1.txt archivo2.txt
  ```

- Numerar todas las líneas:

  ```bash
  cat -n archivo.txt
  ```

- Mostrar el final de cada línea con `$`:

  ```bash
  cat -E archivo.txt
  ```

