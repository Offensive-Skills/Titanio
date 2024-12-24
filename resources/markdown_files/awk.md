### **Básico/Procesamiento de Texto/awk.md**

# awk

## Descripción

`awk` es un lenguaje de programación para procesamiento y análisis de texto, especialmente útil para manipular archivos estructurados por campos.

## Uso

```bash
awk 'programa' archivo
```

### Opciones principales

- `-F`: Especifica el delimitador de campo.
- `-v`: Asigna valor a una variable dentro del programa `awk`.
- `-f`: Ejecuta un programa `awk` desde un archivo.

## Ejemplos

- Imprimir la primera columna de un archivo separado por espacios:

  ```bash
  awk '{print $1}' archivo.txt
  ```

- Usar un delimitador personalizado, como una coma:

  ```bash
  awk -F, '{print $2}' archivo.csv
  ```

- Filtrar y sumar una columna específica:

  ```bash
  awk '{sum += $3} END {print sum}' archivo.txt
  ```

- Imprimir líneas que cumplen una condición:

  ```bash
  awk '$3 > 100 {print $1, $2}' archivo.txt
  ```
