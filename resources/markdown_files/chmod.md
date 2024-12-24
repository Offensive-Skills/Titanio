### **Básico/Gestión de Archivos/chmod.md**

# chmod

## Descripción

`chmod` cambia los permisos de acceso de archivos y directorios.

## Uso

```bash
chmod [opciones] modo archivo
```

### Opciones principales

- `-R`: Aplica los cambios de forma recursiva a directorios.
- `-v`: Modo detallado, muestra las acciones realizadas.
- `--reference=archivo_referencia`: Aplica los permisos del archivo de referencia.

### Modos comunes

- Numéricos:
  - `755`: rwxr-xr-x
  - `644`: rw-r--r--
- Simbólicos:
  - `u+x`: Añade ejecución para el usuario.
  - `go-w`: Quita escritura para grupo y otros.

## Ejemplos

- Dar permisos de lectura, escritura y ejecución al propietario, y solo lectura y ejecución al grupo y otros:

  ```bash
  chmod 755 script.sh
  ```

- Añadir permiso de ejecución para el usuario:

  ```bash
  chmod u+x archivo.sh
  ```

- Quitar permisos de escritura para grupo y otros:

  ```bash
  chmod go-w archivo.txt
  ```

- Cambiar permisos recursivamente en un directorio:

  ```bash
  chmod -R 755 carpeta/
  ```