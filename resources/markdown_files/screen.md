### **Básico/Miscelánea/screen.md**

# screen

## Descripción

`screen` es un multiplexor de terminal que permite tener múltiples sesiones en una sola ventana de terminal.

## Uso

screen [opciones] [comando]

### Opciones principales

- `-S nombre`: Crea una nueva sesión con nombre.
- `-ls`: Lista sesiones existentes.
- `-r`: Reanuda una sesión detenida.

## Ejemplos

- Iniciar una nueva sesión:

  screen

- Crear una sesión con nombre:

  screen -S mi_sesion

- Reanudar una sesión:

  screen -r mi_sesion
