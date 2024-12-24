### **Básico/Procesamiento de Texto/grep.md**

# grep

## Descripción

`grep` busca patrones en el contenido de archivos.

## Uso

```bash
grep [opciones] patrón archivo
```

### Opciones principales

- `-i`: Ignora mayúsculas y minúsculas.
- `-r` o `-R`: Busca recursivamente en directorios.
- `-v`: Invierte la búsqueda, mostrando líneas que no coinciden.
- `-n`: Muestra el número de línea donde se encontró el patrón.
- `-c`: Muestra solo el conteo de coincidencias por archivo.
- `-E`: Usa expresiones regulares extendidas.
- `-l`: Muestra solo los nombres de archivos que contienen el patrón.

## Ejemplos

- Buscar una palabra en un archivo:

  ```bash
  grep "error" archivo.log
  ```

- Buscar ignorando mayúsculas:

  ```bash
  grep -i "Error" archivo.log
  ```

- Buscar recursivamente en un directorio:

  ```bash
  grep -r "función" /ruta/del/directorio/
  ```

- Mostrar líneas que no contienen el patrón:

  ```bash
  grep -v "excluir" archivo.txt
  ```

- Mostrar el número de línea de las coincidencias:

  ```bash
  grep -n "buscar" archivo.txt
  ```
