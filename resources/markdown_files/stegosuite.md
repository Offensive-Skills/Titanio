### **Esteganografía/Herramientas de Ocultación de Datos/Stegosuite.md**

# Stegosuite

## Descripción

`Stegosuite` es una aplicación gráfica de esteganografía que facilita la ocultación y extracción de datos en archivos multimedia como imágenes y audio. Ofrece una interfaz intuitiva para usuarios que prefieren no trabajar con la línea de comandos.

## Uso

```bash
stegosuite
```

### Opciones principales

- `Ocultar datos`: Permite seleccionar un archivo portador y el archivo que se desea ocultar.
- `Extraer datos`: Permite seleccionar un archivo portador para extraer los datos ocultos.
- `Opciones de cifrado`: Configura la contraseña y métodos de cifrado para proteger los datos ocultos.
- `Configuración de compresión`: Establece el nivel de compresión antes de ocultar los datos.
- `Vista previa`: Muestra una vista previa del archivo portador con los datos ocultos.

## Ejemplos

- **Ocultar datos:**
  1. Abrir Stegosuite.
  2. Seleccionar "Ocultar datos".
  3. Elegir el archivo portador (ej., imagen.png).
  4. Seleccionar el archivo a ocultar (ej., secreto.txt).
  5. Introducir una contraseña y ajustar las opciones de cifrado si es necesario.
  6. Guardar el archivo portador modificado.

- **Extraer datos:**
  1. Abrir Stegosuite.
  2. Seleccionar "Extraer datos".
  3. Elegir el archivo portador con los datos ocultos (ej., imagen_oculta.png).
  4. Introducir la contraseña utilizada para ocultar los datos.
  5. Guardar el archivo extraído.
