### **Básico/Procesamiento de Texto/sort.md**

# sort

## Descripción

`sort` ordena las líneas de texto en archivos o entrada estándar.

## Uso

```bash
sort [opciones] archivo
```

### Opciones principales

- `-n`: Ordena numéricamente.
- `-r`: Ordena en orden inverso.
- `-u`: Elimina líneas duplicadas.
- `-k`: Especifica la clave de ordenamiento.
- `-t`: Define el delimitador de campo.
- `-o`: Especifica un archivo de salida.

## Ejemplos

- Ordenar alfabéticamente:

  ```bash
  sort archivo.txt
  ```

- Ordenar numéricamente:

  ```bash
  sort -n archivo.txt
  ```

- Ordenar en orden inverso:

  ```bash
  sort -r archivo.txt
  ```

- Ordenar y eliminar duplicados:

  ```bash
  sort -u archivo.txt
  ```

- Ordenar por el segundo campo, delimitado por coma:

  ```bash
  sort -t',' -k2 archivo.csv
  ```
