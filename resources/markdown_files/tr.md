### **Básico/Procesamiento de Texto/tr.md**


# tr

## Descripción

`tr` traduce o elimina caracteres de la entrada estándar y escribe el resultado en la salida estándar.

## Uso

```bash
tr [opciones] SET1 [SET2]
```

### Opciones principales

- `-d`: Elimina los caracteres especificados.
- `-s`: Suprime repeticiones de los caracteres especificados.
- `-c`: Complementa el conjunto de caracteres.
- `-t`: Trunca el último conjunto al tamaño del primero.

## Ejemplos

- Convertir texto a mayúsculas:

  ```bash
  echo "texto" | tr 'a-z' 'A-Z'
  ```

- Eliminar dígitos de una cadena:

  ```bash
  echo "abc123" | tr -d '0-9'
  ```

- Suprimir caracteres repetidos:

  ```bash
  echo "aabbcc" | tr -s 'a-c'
  ```

- Reemplazar espacios por guiones:

  ```bash
  echo "hola mundo" | tr ' ' '-'
  ```