### **Básico/Miscelánea/ps.md**

# ps

## Descripción

`ps` muestra una lista de procesos en ejecución.

## Uso

ps [opciones]

### Opciones principales

- `-e`: Muestra todos los procesos.
- `-f`: Muestra información completa.
- `-u usuario`: Muestra procesos de un usuario específico.
- `-aux`: Muestra todos los procesos en formato extendido.

## Ejemplos

- Mostrar todos los procesos:

  ps -e

- Mostrar procesos con información detallada:

  ps -ef

- Mostrar procesos de un usuario:

  ps -u usuario
