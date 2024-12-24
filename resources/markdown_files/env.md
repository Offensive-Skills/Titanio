### **Básico/Miscelánea/env.md**

# env

## Descripción

`env` muestra o modifica el entorno de la sesión actual, y puede ejecutar comandos en un entorno modificado.

## Uso

env [opciones] [VARIABLE=valor] [comando]

### Opciones principales

- `-i`: Inicia con un entorno vacío.
- `-u`: Elimina una variable de entorno.
- `--help`: Muestra ayuda sobre el comando.
- `--version`: Muestra la versión de `env`.

## Ejemplos

- Mostrar las variables de entorno actuales:

  env

- Ejecutar un comando con una variable de entorno modificada:

  env VAR=valor comando

- Eliminar una variable de entorno y ejecutar un comando:

  env -u VAR comando
