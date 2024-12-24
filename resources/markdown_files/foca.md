### **Miscelánea/Recolección de Información/FOCA.md**

# FOCA

## Descripción

`FOCA` (Fingerprinting Organizations with Collected Archives) es una herramienta de reconocimiento que analiza metadatos y propiedades ocultas en documentos públicos como PDFs, DOCs, y presentaciones. Extrae información sensible como nombres de usuario, rutas de archivos y versiones de software utilizadas.

## Uso

```bash
foca [opciones]
```

### Opciones principales

- `-d`, `--domain`: Dominio objetivo para la recolección de documentos.
- `-c`, `--crawling`: Inicia un rastreo de documentos en el sitio web.
- `-m`, `--metadata`: Extrae metadatos de los documentos recolectados.
- `-o`, `--output`: Directorio para guardar los resultados.
- `-p`, `--proxy`: Configura un proxy para las solicitudes.
- `-h`, `--help`: Muestra la ayuda y opciones disponibles.

## Ejemplos

- Rastrear y analizar documentos en el dominio ejemplo.com:
  
  ```bash
  foca -d ejemplo.com -c -m -o resultados/
  ```

- Extraer metadatos de documentos específicos:
  
  ```bash
  foca -m -o metadatos/ documentos/*.pdf
  ```

- Utilizar un proxy para las solicitudes:
  
  ```bash
  foca -d ejemplo.com -c -m -o resultados/ -p http://proxy:8080
  ```
