### **Básico/Gestión de Archivos/touch.md**


# touch

## Descripción

`touch` actualiza las marcas de tiempo de un archivo o crea un archivo vacío si no existe.

## Uso

```bash
touch [opciones] archivo
```

### Opciones principales

- `-c` o `--no-create`: No crea el archivo si no existe.
- `-a`: Actualiza solo la marca de tiempo de acceso.
- `-m`: Actualiza solo la marca de tiempo de modificación.
- `-t`: Especifica una marca de tiempo personalizada.

## Ejemplos

- Crear un archivo vacío:

  ```bash
  touch archivo.txt
  ```

- Actualizar solo la marca de tiempo de modificación:

  ```bash
  touch -m archivo.txt
  ```

- Crear múltiples archivos:

  ```bash
  touch archivo1.txt archivo2.txt archivo3.txt
  ```

- No crear el archivo si no existe:

  ```bash
  touch -c archivo.txt
  ```
