### **Básico/Procesamiento de Texto/cut.md**

# cut

## Descripción

`cut` extrae secciones de cada línea de un archivo o entrada estándar.

## Uso

```bash
cut [opciones] archivo
```

### Opciones principales

- `-f`: Especifica los campos a extraer.
- `-d`: Define el delimitador de campo (por defecto es tabulación).
- `-c`: Especifica los rangos de caracteres a extraer.
- `--complement`: Extrae todos los campos excepto los especificados.

## Ejemplos

- Extraer el primer campo separado por comas:

  ```bash
  cut -d',' -f1 archivo.csv
  ```

- Extraer los caracteres del 1 al 5 de cada línea:

  ```bash
  cut -c1-5 archivo.txt
  ```

- Extraer múltiples campos:

  ```bash
  cut -d':' -f1,3 archivo.txt
  ```

- Extraer todos los campos excepto el segundo:

  ```bash
  cut --complement -f2 archivo.txt
  ```