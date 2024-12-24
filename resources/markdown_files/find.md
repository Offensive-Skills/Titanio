### **Básico/Miscelánea/find.md**

# find

## Descripción

`find` busca archivos y directorios en una jerarquía de directorios basándose en condiciones específicas.

## Uso

find [ruta] [condiciones]

### Opciones principales

- `-name`: Busca por nombre de archivo.
- `-type`: Busca por tipo (f: archivo, d: directorio).
- `-size`: Busca por tamaño.
- `-mtime`: Busca por fecha de modificación.
- `-exec`: Ejecuta un comando en los archivos encontrados.
- `-user`: Busca por propietario.

## Ejemplos

- Buscar archivos llamados "archivo.txt":

  find /ruta -name "archivo.txt"

- Buscar archivos mayores de 10 MB:

  find /ruta -size +10M

- Buscar archivos modificados en los últimos 2 días:

  find /ruta -mtime -2

- Eliminar archivos con extensión ".tmp":

  find /ruta -name "*.tmp" -exec rm {} \;
