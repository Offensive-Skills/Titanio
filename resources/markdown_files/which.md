### **Básico/Miscelánea/which.md**

# which

## Descripción

`which` muestra la ruta completa de los comandos ejecutables en el PATH.

## Uso

which [opciones] comando

### Opciones principales

- `-a`: Muestra todas las ubicaciones encontradas en el PATH.
- `--skip-alias`: Ignora los alias.
- `--skip-functions`: Ignora funciones de shell.

## Ejemplos

- Encontrar la ruta de `python`:

  which python

- Mostrar todas las ubicaciones de `ls`:

  which -a ls
