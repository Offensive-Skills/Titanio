### **Análisis y Extracción/zsteg.md**

# zsteg

## Descripción

`zsteg` es una herramienta de esteganografía diseñada para detectar y extraer datos ocultos en archivos PNG e imágenes BMP. Es especialmente útil para encontrar datos ocultos mediante técnicas como la manipulación de bits o la inserción de datos en los canales de color.

## Uso

```bash
zsteg [opciones] archivo
```

### Opciones principales

- `-a`: Activa todas las técnicas de detección disponibles.
- `-E`: Especifica expresiones regulares para filtrar resultados.
- `-x`: Extrae los datos ocultos en un formato específico.
- `-f`: Filtra los resultados basados en patrones de datos.
- `-p`: Define el formato de salida para los datos extraídos.
- `--help`: Muestra ayuda y opciones disponibles.

## Ejemplos

- Analizar una imagen PNG en busca de datos ocultos utilizando todas las técnicas:

  ```bash
  zsteg -a imagen.png
  ```

- Extraer datos ocultos específicos de una imagen:

  ```bash
  zsteg -x "data" imagen.png
  ```

- Filtrar resultados con una expresión regular:

  ```bash
  zsteg -E "regex" imagen.png
  ```

- Definir el formato de salida para los datos extraídos:

  ```bash
  zsteg -p hex imagen.png
  ```

- Mostrar solo las coincidencias que contienen una palabra clave:

  ```bash
  zsteg --grep "clave" imagen.png
  ```
