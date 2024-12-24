### **Análisis y Extracción/Stegdetect.md**

# Stegdetect

## Descripción

`Stegdetect` es una herramienta de detección de esteganografía que analiza archivos de imagen en busca de firmas conocidas de técnicas de ocultación de datos. Es útil para identificar si una imagen contiene información oculta mediante métodos específicos.

## Uso

```bash
stegdetect [opciones] archivo
```

### Opciones principales

- `-v`: Modo verbose, muestra información detallada durante el análisis.
- `-f`: Define un archivo de firmas personalizado.
- `-s`: Salida silenciosa, muestra solo resultados relevantes.
- `--help`: Muestra ayuda y opciones disponibles.

## Ejemplos

- Analizar una imagen en busca de firmas de esteganografía:

  ```bash
  stegdetect imagen.png
  ```

- Analizar una imagen con un archivo de firmas personalizado:

  ```bash
  stegdetect -f firmas_personalizadas.sig imagen.png
  ```

- Ejecutar el análisis en modo verbose para obtener más detalles:

  ```bash
  stegdetect -v imagen.png
  ```

- Analizar múltiples imágenes a la vez:

  ```bash
  stegdetect imagen1.png imagen2.png imagen3.png
  ```

**Nota:** `Stegdetect` es más eficaz cuando las firmas de esteganografía están definidas en su base de datos de firmas. Para detectar técnicas personalizadas, se requiere un archivo de firmas adecuado.
