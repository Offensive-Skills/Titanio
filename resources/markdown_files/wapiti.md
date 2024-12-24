### **Hacking Web/Escáneres de Vulnerabilidades Web/Wapiti.md**

# Wapiti

## Descripción

`Wapiti` es una herramienta de escaneo de vulnerabilidades web de código abierto que permite identificar fallos de seguridad en aplicaciones web. Realiza análisis de inyección SQL, Cross-Site Scripting (XSS), y otros tipos de vulnerabilidades, generando reportes detallados para facilitar la remediación.

## Uso

```bash
wapiti [opciones]
```

### Opciones principales

- `-u URL`: Especifica la URL objetivo para el escaneo.
- `-f FORMAT`: Define el formato del reporte (e.g., html, xml, json).
- `-o OUTPUT`: Especifica el archivo donde se guardará el reporte.
- `--scope SCOPE`: Define el alcance del escaneo (e.g., all, external).
- `--attack ATTACK_TYPE`: Selecciona el tipo de ataques a realizar (e.g., sql, xss).
- `--recursive`: Realiza un escaneo recursivo en la aplicación.
- `--proxy PROXY_URL`: Usa un proxy específico durante el escaneo.
- `--help`: Muestra ayuda sobre las opciones disponibles.

## Ejemplos

- Realizar un escaneo básico en una URL y generar un reporte en HTML:
  
  ```bash
  wapiti -u "http://example.com" -f html -o reporte_wapiti.html
  ```

- Realizar un escaneo recursivo con ataques SQL y XSS:
  
  ```bash
  wapiti -u "http://example.com" --attack sql,xss --recursive
  ```

- Generar un reporte en formato JSON:
  
  ```bash
  wapiti -u "http://example.com" -f json -o reporte_wapiti.json
  ```

- Usar un proxy específico durante el escaneo:
  
  ```bash
  wapiti -u "http://example.com" --proxy "http://127.0.0.1:8080"
  ```

