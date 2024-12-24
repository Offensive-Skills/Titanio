### **Básico/Gestión de Archivos/stat.md**

# stat

## Descripción

`stat` muestra información detallada sobre archivos y directorios.

## Uso

```bash
stat [opciones] archivo
```

### Opciones principales

- `-c` o `--format=FORMATO`: Especifica el formato de salida.
- `-t`: Salida breve, adecuada para scripts.
- `--printf=FORMATO`: Similar a `-c` pero sin un salto de línea al final.

## Ejemplos

- Mostrar información detallada de un archivo:

  ```bash
  stat archivo.txt
  ```

- Mostrar solo el tamaño del archivo:

  ```bash
  stat -c%s archivo.txt
  ```

- Mostrar la fecha de última modificación:

  ```bash
  stat -c%y archivo.txt
  ```

- Usar un formato personalizado:

  ```bash
  stat --format="Archivo: %n%nTamaño: %s bytes%nModificado: %y" archivo.txt
  ```