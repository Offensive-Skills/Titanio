### **Debugging/Strace/strace.md**

# Strace

## Descripción

`strace` es una herramienta de línea de comandos utilizada para rastrear las llamadas al sistema y las señales recibidas por un programa durante su ejecución. Es invaluable para la depuración, análisis de rendimiento y resolución de problemas en aplicaciones, permitiendo a los desarrolladores observar la interacción del programa con el sistema operativo.

## Uso

```bash
strace [opciones] comando [argumentos]
```

### Opciones principales

- `-o archivo_salida`: Guarda la salida de strace en un archivo.
- `-e expresión`: Filtra las llamadas al sistema por categoría o nombre.
- `-f`: Sigue los procesos hijos creados por el programa.
- `-c`: Muestra un resumen de las llamadas al sistema y su tiempo.
- `-s tamaño`: Define el tamaño máximo de las cadenas de texto a mostrar.
- `-p pid`: Adjunta strace a un proceso ya en ejecución mediante su PID.

### Opciones de filtrado comunes

- `file`: Rastrea llamadas relacionadas con archivos (e.g., open, read, write).
- `network`: Rastrea llamadas de red (e.g., socket, connect).
- `process`: Rastrea llamadas de gestión de procesos (e.g., fork, exec).

## Ejemplos

- Rastrear todas las llamadas al sistema de un programa:

  ```bash
  strace ./mi_programa
  ```

- Guardar el rastreo en un archivo:

  ```bash
  strace -o rastreo.txt ./mi_programa
  ```

- Filtrar y rastrear solo llamadas relacionadas con archivos:

  ```bash
  strace -e trace=file ./mi_programa
  ```

- Adjuntar strace a un proceso en ejecución con PID 1234:

  ```bash
  strace -p 1234
  ```

- Mostrar un resumen de las llamadas al sistema y su frecuencia:

  ```bash
  strace -c ./mi_programa
  ```

