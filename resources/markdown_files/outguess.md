### **Esteganografía/Herramientas de Ocultación de Datos/OutGuess.md**

# OutGuess

## Descripción

`OutGuess` es una herramienta de esteganografía que permite ocultar datos de manera imperceptible dentro de archivos de medios como imágenes. Ofrece opciones avanzadas para minimizar la detección mediante análisis estadísticos.

## Uso

```bash
outguess [opciones] archivo_portador archivo_oculto archivo_salida
```

### Opciones principales

- `-k`: Define una clave de cifrado para proteger los datos ocultos.
- `-d`: Extrae los datos ocultos de un archivo portador.
- `-r`: Realiza una rotación de bits para mejorar la imperceptibilidad.
- `-c`: Utiliza un archivo de configuración para parámetros avanzados.
- `-p`: Preserva los metadatos del archivo portador.

## Ejemplos

- Ocultar un archivo dentro de una imagen con una clave:

  ```bash
  outguess -k contraseña secreto.txt imagen.jpg imagen_oculta.jpg
  ```

- Extraer un archivo oculto de una imagen:

  ```bash
  outguess -k contraseña -r imagen_oculta.jpg datos_extraidos.txt
  ```

- Ocultar un archivo sin cifrado:

  ```bash
  outguess -k "" secreto.txt imagen.jpg imagen_oculta.jpg
  ```

