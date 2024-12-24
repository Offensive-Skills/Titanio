### **Básico/Miscelánea/su.md**

# su

## Descripción

`su` cambia el usuario efectivo en la sesión actual, iniciando una nueva shell.

## Uso

su [opciones] [usuario]

### Opciones principales

- `-`: Inicia una shell de inicio de sesión.
- `-c`: Ejecuta un comando específico.
- `-m` o `-p`: Mantiene el entorno del usuario actual.

## Ejemplos

- Cambiar al usuario root:

  su -

- Cambiar a otro usuario sin cambiar el entorno:

  su usuario

- Ejecutar un comando como otro usuario:

  su -c "comando" usuario
