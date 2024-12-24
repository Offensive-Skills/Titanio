### **Básico/Miscelánea/locate.md**

# locate

## Descripción

`locate` busca archivos en una base de datos indexada, proporcionando resultados rápidos.

## Uso

locate [opciones] patrón

### Opciones principales

- `-i`: Ignora mayúsculas y minúsculas.
- `-r`: Utiliza expresiones regulares.
- `-n`: Limita el número de resultados.
- `-e`: Verifica que los archivos existan realmente.

## Ejemplos

- Buscar archivos que contengan "documento":

  locate documento

- Buscar ignorando mayúsculas:

  locate -i Documento

- Limitar resultados a 5 archivos:

  locate -n 5 archivo

- Actualizar la base de datos de `locate`:

  sudo updatedb
