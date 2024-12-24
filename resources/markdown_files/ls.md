### **Básico/Gestión de Archivos/ls.md**

# ls

## Descripción

`ls` lista los archivos y directorios en el directorio actual o en una ruta especificada.

## Uso

```bash
ls [opciones] [ruta]
```

### Opciones principales

- `-l`: Formato largo, muestra permisos, propietario, tamaño y fecha.
- `-a`: Muestra todos los archivos, incluidos los ocultos (que comienzan con `.`).
- `-h`: Tamaños legibles (e.g., K, M).
- `-R`: Lista directorios de forma recursiva.
- `-t`: Ordena por fecha de modificación, mostrando los más recientes primero.

## Ejemplos

- Listar archivos en formato largo:

  ```bash
  ls -l
  ```

- Listar todos los archivos, incluidos los ocultos:

  ```bash
  ls -a
  ```

- Listar archivos con tamaños legibles:

  ```bash
  ls -lh
  ```

- Listar directorios de forma recursiva:

  ```bash
  ls -R
  ```

