### **Análisis Forense/LiME/lime.md**

# LiME

## Descripción

**LiME (Linux Memory Extractor)** es un módulo de kernel para Linux que permite capturar el contenido de la memoria RAM completa de un sistema. Es útil para realizar análisis forense de memoria en sistemas Linux.

## Uso

LiME se carga como un módulo del kernel y se especifican parámetros al cargarlo.

### Opciones principales

- `path`: Especifica la ruta y nombre del archivo donde se almacenará el volcado.
- `format`: Define el formato de salida (raw, lime).
- `pid`: (Opcional) Volca solo la memoria asociada a un PID específico.

## Ejemplos

- Compilar el módulo:

  ```bash
  make
  ```

- Cargar el módulo y volcar la memoria:

  ```bash
  insmod lime.ko "path=/ruta/memoria.lime format=lime"
  ```

- Descargar el módulo después de la captura:

  ```bash
  rmmod lime
  ```


