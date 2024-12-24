### **Básico/Procesamiento de Texto/sed.md**


# sed

## Descripción

`sed` es un editor de flujo que realiza transformaciones de texto en un flujo de datos o archivo.

## Uso

```bash
sed [opciones] 'comando' archivo
```

### Opciones principales

- `-i`: Edita los archivos en el lugar.
- `-e`: Permite especificar múltiples comandos.
- `-n`: Suprime la salida automática, útil con el comando `p`.
- `s`: Sustitución de texto.
- `d`: Elimina líneas que coinciden con el patrón.
- `p`: Imprime líneas que coinciden con el patrón.

## Ejemplos

- Reemplazar la primera ocurrencia de "foo" por "bar" en cada línea:

  ```bash
  sed 's/foo/bar/' archivo.txt
  ```

- Reemplazar todas las ocurrencias de "foo" por "bar":

  ```bash
  sed 's/foo/bar/g' archivo.txt
  ```

- Eliminar líneas que contienen "error":

  ```bash
  sed '/error/d' archivo.txt
  ```

- Reemplazar texto en el archivo original:

  ```bash
  sed -i 's/old/new/g' archivo.txt
  ```

- Usar múltiples comandos:

  ```bash
  sed -e 's/foo/bar/' -e '/error/d' archivo.txt
  ```

