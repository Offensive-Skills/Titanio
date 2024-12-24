### **Básico/Miscelánea/date.md**

# date

## Descripción

`date` muestra o establece la fecha y hora del sistema.

## Uso

date [opciones] [+formato]

### Opciones principales

- `-u`: Muestra la hora en UTC.
- `-s`: Establece la fecha y hora.
- `+%Y-%m-%d`: Formato personalizado de fecha.

## Ejemplos

- Mostrar la fecha y hora actuales:

  date

- Mostrar solo la fecha:

  date "+%Y-%m-%d"

- Establecer la fecha y hora (requiere permisos):

  sudo date -s "2023-10-01 12:34:56"
