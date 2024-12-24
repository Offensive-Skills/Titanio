### **Básico/Procesamiento de Texto/tail.md**

# tail

## Descripción

`tail` muestra las últimas líneas de un archivo y puede seguir el crecimiento de un archivo en tiempo real.

## Uso

```bash
tail [opciones] archivo
```

### Opciones principales

- `-n`: Especifica el número de líneas a mostrar.
- `-c`: Muestra el número de bytes.
- `-f`: Sigue el archivo en tiempo real, mostrando nuevas líneas a medida que se agregan.
- `-F`: Similar a `-f` pero intenta reconectar si el archivo se renombra.
- `-q`: Suprime los encabezados de los archivos.
- `-v`: Siempre muestra los encabezados.

## Ejemplos

- Mostrar las últimas 10 líneas (por defecto):

  ```bash
  tail archivo.log
  ```

- Mostrar las últimas 20 líneas:

  ```bash
  tail -n 20 archivo.log
  ```

- Seguir un archivo en tiempo real:

  ```bash
  tail -f archivo.log
  ```

- Mostrar las últimas 50 líneas y seguir el archivo:

  ```bash
  tail -n 50 -f archivo.log
  ```
