### **Básico/Procesamiento de Texto/less.md**

# less

## Descripción

`less` es un visualizador de archivos que permite navegar hacia adelante y hacia atrás.

## Uso

```bash
less [opciones] archivo
```

### Opciones principales

- `-N`: Muestra números de línea.
- `-S`: No envuelve las líneas largas.
- `-R`: Muestra códigos de color.
- `-F`: Sale si el contenido cabe en una pantalla.
- `-X`: No limpia la pantalla al salir.

### Controles de navegación

- `Espacio`: Avanza una página.
- `b`: Retrocede una página.
- `/patrón`: Busca hacia adelante el patrón.
- `?patrón`: Busca hacia atrás el patrón.
- `n`: Repite la última búsqueda hacia adelante.
- `N`: Repite la última búsqueda hacia atrás.
- `q`: Sale de `less`.

## Ejemplos

- Visualizar un archivo con números de línea:

  ```bash
  less -N archivo.txt
  ```

- Visualizar sin envolver líneas largas:

  ```bash
  less -S archivo.txt
  ```

- Visualizar con soporte de colores:

  ```bash
  less -R archivo_coloreado.txt
  ```
