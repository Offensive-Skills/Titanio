### **Análisis Forense/The Sleuth Kit/sleuth_kit.md**

# The Sleuth Kit

## Descripción

**The Sleuth Kit (TSK)** es una colección de herramientas de línea de comandos para realizar análisis forense de sistemas de archivos. Permite examinar particiones, sistemas de archivos y recuperar datos eliminados, siendo una base para muchas otras herramientas forenses como Autopsy.

## Uso

Las herramientas de TSK se ejecutan desde la línea de comandos y cada una tiene funciones específicas.

### Herramientas principales

- `fls`: Lista archivos y directorios en una imagen.
- `icat`: Extrae archivos por número de inodo.
- `istat`: Muestra información detallada de un inodo.
- `dd`: Copia datos de una imagen o dispositivo.
- `fsstat`: Muestra estadísticas del sistema de archivos.
- `blkls`: Extrae contenido no asignado y espacio libre.

## Ejemplos

- Listar archivos y directorios:

  ```bash
  fls -r imagen.dd
  ```

- Extraer un archivo específico:

  ```bash
  icat imagen.dd 128 > archivo_extraido.txt
  ```

- Ver información de un inodo:

  ```bash
  istat imagen.dd 128
  ```
