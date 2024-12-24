### **Esteganografía/Herramientas de Ocultación de Datos/SilentEye.md**

# SilentEye

## Descripción

`SilentEye` es una herramienta de esteganografía con interfaz gráfica que facilita la ocultación de archivos dentro de imágenes y archivos de audio. Ofrece opciones de cifrado y compresión para proteger y optimizar los datos ocultos.

## Uso

```bash
silenteye
```

### Opciones principales

- `Ocultar archivo`: Permite seleccionar el archivo portador y el archivo a ocultar.
- `Extraer archivo`: Permite seleccionar el archivo portador para extraer los datos ocultos.
- `Opciones de cifrado`: Configura la contraseña y el algoritmo de cifrado para los datos ocultos.
- `Opciones de compresión`: Ajusta el nivel de compresión antes de ocultar los datos.
- `Vista previa`: Muestra una vista previa del archivo portador con los datos ocultos.

## Ejemplos

- **Ocultar un archivo:**
  1. Abrir SilentEye.
  2. Seleccionar "Ocultar archivo".
  3. Elegir el archivo portador (ej., imagen.png).
  4. Seleccionar el archivo a ocultar (ej., secreto.txt).
  5. Introducir una contraseña y configurar las opciones de cifrado si es necesario.
  6. Guardar el archivo portador modificado.

- **Extraer un archivo:**
  1. Abrir SilentEye.
  2. Seleccionar "Extraer archivo".
  3. Elegir el archivo portador con los datos ocultos (ej., imagen_oculta.png).
  4. Introducir la contraseña utilizada para ocultar los datos.
  5. Guardar el archivo extraído.
