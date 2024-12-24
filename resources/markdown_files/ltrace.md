### **Debugging/Ltrace/ltrace.md**

# Ltrace

## Descripción

`ltrace` es una herramienta de línea de comandos para rastrear llamadas a funciones de bibliotecas dinámicas realizadas por un programa durante su ejecución. Permite observar cómo un programa interactúa con las bibliotecas del sistema, facilitando la detección de errores y el análisis del comportamiento del software.

## Uso

```bash
ltrace [opciones] comando [argumentos]
```

### Opciones principales

- `-e expresion`: Filtra las llamadas a funciones que coinciden con la expresión.
- `-o archivo_salida`: Guarda la salida de ltrace en un archivo.
- `-c`: Muestra un resumen de las llamadas a funciones y su frecuencia.
- `-s tamaño`: Define el tamaño máximo de las cadenas de texto a mostrar.
- `-f`: Sigue los procesos hijos creados por el programa.

## Ejemplos

- Rastrear todas las llamadas a funciones de un programa:

  ```bash
  ltrace ./mi_programa
  ```

- Filtrar y rastrear solo las llamadas a funciones `malloc` y `free`:

  ```bash
  ltrace -e malloc,free ./mi_programa
  ```

- Guardar el registro de llamadas a funciones en un archivo:

  ```bash
  ltrace -o llamadas.txt ./mi_programa
  ```

- Mostrar un resumen de las llamadas a funciones:

  ```bash
  ltrace -c ./mi_programa
  ```

- Rastrear llamadas en un programa que crea procesos hijos:

  ```bash
  ltrace -f ./mi_programa
  ```
