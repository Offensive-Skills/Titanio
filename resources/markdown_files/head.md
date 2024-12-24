### **Básico/Procesamiento de Texto/head.md**

# head

## Descripción

`head` muestra las primeras líneas de un archivo.

## Uso

```bash
head [opciones] archivo
```

### Opciones principales

- `-n`: Especifica el número de líneas a mostrar.
- `-c`: Muestra el número de bytes.
- `-q`: Suprime los encabezados de los archivos.
- `-v`: Siempre muestra los encabezados.

## Ejemplos

- Mostrar las primeras 10 líneas (por defecto):

  ```bash
  head archivo.txt
  ```

- Mostrar las primeras 5 líneas:

  ```bash
  head -n 5 archivo.txt
  ```

- Mostrar los primeros 100 bytes:

  ```bash
  head -c 100 archivo.txt
  ```

- Mostrar las primeras 15 líneas de múltiples archivos:

  ```bash
  head -n 15 archivo1.txt archivo2.txt
  ```