### **Análisis Forense/Foremost/foremost.md**

# Foremost

## Descripción

`foremost` es una herramienta de recuperación de datos diseñada para extraer archivos basados en sus encabezados, pies de página y estructuras internas. Es útil para recuperar archivos borrados de discos duros, imágenes y otros medios.

## Uso

```bash
foremost [opciones] -i archivo_entrada -o directorio_salida
```

### Opciones principales

- `-i`: Especifica el archivo de entrada (dispositivo o imagen).
- `-o`: Define el directorio donde se guardarán los archivos recuperados.
- `-t`: Especifica los tipos de archivos a extraer (ej. jpg,png,doc).
- `-c`: Utiliza un archivo de configuración personalizado.
- `-v`: Modo detallado.

## Ejemplos

- Recuperar todos los tipos de archivos:

  ```bash
  foremost -i imagen.dd -o salida
  ```

- Recuperar solo imágenes JPEG y PNG:

  ```bash
  foremost -t jpg,png -i imagen.dd -o salida
  ```
