### **Básico/Miscelánea/man.md**

# man

## Descripción

`man` muestra las páginas del manual para comandos y programas.

## Uso

man [opciones] comando

### Opciones principales

- `-k`: Busca en los manuales por palabra clave.
- `-f`: Equivalente a `whatis`, muestra descripciones breves.
- `-a`: Muestra todas las páginas coincidentes en todas las secciones.

## Ejemplos

- Ver el manual de `tar`:

  man tar

- Buscar manuales relacionados con "network":

  man -k network

- Mostrar todas las páginas de `printf`:

  man -a printf
