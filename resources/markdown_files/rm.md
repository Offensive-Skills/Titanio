### **Básico/Gestión de Archivos/rm.md**


# rm

## Descripción

`rm` elimina archivos y directorios.

## Uso

```bash
rm [opciones] archivo
```

### Opciones principales

- `-r` o `-R`: Elimina directorios y su contenido de forma recursiva.
- `-f`: Fuerza la eliminación sin solicitar confirmación.
- `-i`: Solicita confirmación antes de eliminar cada archivo.
- `-v`: Modo detallado, muestra las acciones realizadas.

## Ejemplos

- Eliminar un archivo:

  ```bash
  rm archivo.txt
  ```

- Eliminar un directorio de forma recursiva:

  ```bash
  rm -r carpeta/
  ```

- Forzar la eliminación sin confirmación:

  ```bash
  rm -f archivo.txt
  ```

- Eliminar con confirmación para cada archivo:

  ```bash
  rm -i archivo.txt
  ```