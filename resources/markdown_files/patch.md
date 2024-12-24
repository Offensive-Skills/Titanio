### **Básico/Procesamiento de Texto/patch.md**

# patch

## Descripción

`patch` aplica cambios a archivos utilizando diferencias generadas por `diff`.

## Uso

```bash
patch [opciones] archivo < parche.diff
```

### Opciones principales

- `-pN`: Ignora los primeros N directorios en las rutas de los archivos en el parche.
- `-R`: Revierte un parche previamente aplicado.
- `-i archivo_parche`: Especifica el archivo de parche a aplicar.
- `-d directorio`: Cambia al directorio especificado antes de aplicar el parche.
- `--dry-run`: Simula la aplicación del parche sin realizar cambios.

## Ejemplos

- Aplicar un parche desde un archivo:

  ```bash
  patch < cambios.diff
  ```

- Aplicar un parche ignorando los primeros dos directorios en las rutas:

  ```bash
  patch -p2 < cambios.diff
  ```

- Aplicar un parche desde un archivo específico:

  ```bash
  patch -i parche.diff
  ```

- Simular la aplicación de un parche:

  ```bash
  patch --dry-run < cambios.diff
  ```