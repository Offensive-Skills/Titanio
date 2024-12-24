### **Análisis Forense/YARA/yara.md**

# YARA

## Descripción

**YARA** es una herramienta para identificar y clasificar malware mediante la creación de reglas basadas en patrones de texto o binarios. Es ampliamente utilizada en análisis de malware y respuesta a incidentes.

## Uso

```bash
yara [opciones] regla archivo
```

### Opciones principales

- `-r`: Recursivo, analiza directorios y subdirectorios.
- `-s`: Muestra las cadenas que coincidieron.
- `-d`: Define variables externas para las reglas.
- `-k`: Continúa analizando incluso si hay errores.
- `-w`: Ignora advertencias de compilación.

## Ejemplos

- Analizar un archivo con una regla:

  ```bash
  yara regla.yar archivo.bin
  ```

- Analizar un directorio recursivamente:

  ```bash
  yara -r reglas.yar /ruta/directorio
  ```

- Mostrar las cadenas que coincidieron:

  ```bash
  yara -s regla.yar archivo.bin
  ```
