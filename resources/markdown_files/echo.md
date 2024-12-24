### **Básico/Miscelánea/echo.md**

# echo

## Descripción

`echo` muestra una línea de texto en la salida estándar.

## Uso

echo [opciones] [texto]

### Opciones principales

- `-n`: No agrega un salto de línea al final.
- `-e`: Habilita interpretación de secuencias de escape.
- `-E`: Deshabilita interpretación de secuencias de escape.

## Ejemplos

- Mostrar un mensaje en la terminal:

  echo "Hola Mundo"

- Mostrar sin salto de línea:

  echo -n "Sin salto de línea"

- Usar secuencias de escape:

  echo -e "Línea 1\nLínea 2"
