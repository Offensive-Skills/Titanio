### **Básico/Procesamiento de Texto/more.md**

# more

## Descripción

`more` muestra el contenido de un archivo una pantalla a la vez.

## Uso

```bash
more [opciones] archivo
```

### Opciones principales

- `-d`: Muestra mensajes de ayuda más detallados.
- `-c`: Limpia la pantalla en lugar de desplazar.
- `-s`: Suprime líneas en blanco adicionales.
- `/patrón`: Busca hacia adelante el patrón especificado.
- `+n`: Comienza la visualización en la línea n.

## Ejemplos

- Mostrar un archivo paginado:

  ```bash
  more archivo.txt
  ```

- Comenzar en la línea 50:

  ```bash
  more +50 archivo.txt
  ```

- Buscar un patrón mientras se visualiza:

  Presiona `/`, ingresa el patrón y presiona Enter.

