### **Básico/Gestión de Archivos/rmdir.md**


# rmdir

## Descripción

`rmdir` elimina directorios vacíos.

## Uso

```bash
rmdir [opciones] directorio
```

### Opciones principales

- `-p`: Elimina directorios padres si están vacíos.
- `-v`: Modo detallado, muestra las acciones realizadas.

## Ejemplos

- Eliminar un directorio vacío:

  ```bash
  rmdir carpeta_vacia/
  ```

- Eliminar un directorio y sus padres si están vacíos:

  ```bash
  rmdir -p /ruta/a/carpeta/subcarpeta/
  ```

- Eliminar directorios en modo detallado:

  ```bash
  rmdir -v carpeta_vacia/
  ```

