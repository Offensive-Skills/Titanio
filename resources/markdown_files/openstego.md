### **Esteganografía/OpenStego/openstego.md**

# OpenStego

## Descripción

`OpenStego` es una herramienta de esteganografía de código abierto que permite ocultar información dentro de archivos portadores, como imágenes. Es utilizada para proteger la confidencialidad de datos mediante la inserción de mensajes secretos de manera imperceptible.

## Uso

OpenStego proporciona una interfaz gráfica fácil de usar, pero también puede ser operado desde la línea de comandos.

```bash
openstego [opciones]
```

### Opciones principales

- `embed`: Inserta un mensaje oculto en un archivo portador.
- `extract`: Extrae el mensaje oculto de un archivo portador.
- `-cf`: Especifica el archivo portador (cover file).
- `-mf`: Define el mensaje a ocultar (message file).
- `-sf`: Selecciona el archivo de salida para el archivo portador modificado.
- `-sf2`: Define el archivo de salida para el mensaje extraído.

## Ejemplos

- Ocultar un mensaje dentro de una imagen:
  
  ```bash
  openstego embed -cf imagen.png -mf mensaje.txt -sf imagen_oculta.png
  ```

- Extraer el mensaje oculto de una imagen:
  
  ```bash
  openstego extract -cf imagen_oculta.png -sf2 mensaje_extraido.txt
  ```

- Utilizar la interfaz gráfica:
  
  Ejecuta el comando `openstego` sin parámetros para abrir la interfaz y seguir las instrucciones.

