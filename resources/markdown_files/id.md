### **Básico/Miscelánea/id.md**

# id

## Descripción

`id` muestra información sobre el usuario actual o especificado, incluyendo UID, GID y grupos.

## Uso

id [opciones] [usuario]

### Opciones principales

- `-u`: Muestra solo el UID.
- `-g`: Muestra solo el GID.
- `-G`: Muestra todos los GID de los grupos a los que pertenece el usuario.
- `-n`: Muestra los nombres en lugar de los números.
- `-r`: Muestra el ID real en lugar del efectivo.

## Ejemplos

- Mostrar información del usuario actual:

  id

- Mostrar solo el UID:

  id -u

- Mostrar grupos del usuario "juan":

  id juan
