### **Hacking Web/LFI y RCE/RIPS.md**

# RIPS

## Descripción

`RIPS` (Real PHP IDS) es una herramienta de análisis estático diseñada para detectar vulnerabilidades de seguridad en aplicaciones PHP. Automatiza la identificación de fallos como inyecciones SQL, Cross-Site Scripting (XSS) y otros problemas de seguridad, proporcionando reportes detallados para mejorar la seguridad del código.

## Uso

```bash
rips [opciones]
```

### Opciones principales

- `-d DIRECTORY`: Especifica el directorio de la aplicación PHP a analizar.
- `-o OUTPUT`: Define el directorio donde se guardarán los reportes.
- `--format FORMAT`: Define el formato del reporte (HTML, PDF, JSON).
- `--verbose`: Muestra información detallada durante el análisis.
- `--exclude DIR`: Excluye directorios específicos del análisis.
- `--help`: Muestra ayuda sobre las opciones disponibles.

## Ejemplos

- Analizar una aplicación PHP ubicada en el directorio "mi_aplicacion" y guardar el reporte en "reportes":
  
  ```bash
  rips -d /ruta/a/mi_aplicacion -o /ruta/a/reportes
  ```

- Analizar una aplicación y generar un reporte en formato PDF:
  
  ```bash
  rips -d /ruta/a/mi_aplicacion -o /ruta/a/reportes --format PDF
  ```

- Excluir el directorio "vendor" del análisis:
  
  ```bash
  rips -d /ruta/a/mi_aplicacion -o /ruta/a/reportes --exclude /ruta/a/mi_aplicacion/vendor
  ```

- Ejecutar el análisis en modo verbose para obtener más detalles:
  
  ```bash
  rips -d /ruta/a/mi_aplicacion -o /ruta/a/reportes --verbose
  ```
